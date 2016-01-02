.. _npminstall-label:

DreamFace npm Installation Guide
================================

Below are the instructions for installing DreamFace Cloud Application Development Platform using the Node Package Manager npm.




DreamFace is based on the Node.js, Angular.js and MongoDB technologies. It is packaged and installed as three separate Node.js modules:

* **DFX - DreamFace X-Platform** a cloud-based platform used to **develop** and **deploy** web and mobile applications.
* **DFC - DreamFace Compiler** a compiler used to compile and manage different builds of your DreamFace application.
* **DFG - DreamFace Generator** a tool used once during installation to generate development, compiler and deployment environments.

Because of its inherent Cloud nature, DreamFace applications are :term:`multitenant` and each tenant has a dedicated repository
where all application components are stored. All repositories are managed by a MongoDB server. For more information on how DreamFace
handles multitenancy see :ref:`multitenancy-label`

Node.js and MongoDB are therefore the two required elements that need to be installed prior to installing DreamFace.

|

Installing MongoDB
------------------

Download the latest version of MongoDB from http://www.mongodb.org/

Choose the installation that corresponds to your operating system from the downloads page and install it. You can get detailed recommendations on how to install MongoDB on your operating system here: http://docs.mongodb.org/manual/installation/ — For Windows, do the the usual installation from EXE-file, and for Linux or MacOS X this is a standard package installation process.

.. image:: images/installation/dfx-install-mongo.png
	:width: 500px
|

Make sure, that there is a directory for database files in the root directory where you have installed MongoDB. By default, this is “/data/db” at the root of the partition (on Windows) or home directory (on linux systems). If it doesn’t exist, create it manually.
The creation syntax for the command line is described in the guides mentioned above. If your operating system requires permissions for files and folders, set full write permission for this directory.

Then start MongoDB. The file that launches MongoDB is called “mongod” (with “.exe” file extension on Windows) and located in the directory “/bin” in the main directory where MongoDB has been installed.

Below is a summary of steps to install MongoDB as described above:

* Visit http://www.mongodb.org/downloads and download MongoDB for your operating system
* Unpack the downloaded archive to a directory you prefer, e.g. “c:\mongodb”
* Go back to the root or home level directory and create a folder “data/db” there; this directory will contain the databases
* Run MongoDB: launch the file “mongod.exe” in the /bin directory of the MongoDB installation

The DreamFace Repository will be initialized automatically the first time you start the DreamFace application.

|
|

Install Node.js
---------------

Download the latest version of Node.js from http://nodejs.org/ and install it (choose “Install” button for the automatically selected installation package or “Downloads” to select the package manually). Launch usual installation, and when it finishes, go to the directory where Node.js has been installed.

.. image:: images/installation/dfx-install-node-js.png

Summary of the steps to install node.js:

* Visit http://nodejs.org/ and press the button “Install” to download the version of installer which corresponding to your operating system.
* Start installation Node.js. Please change default installation path to another to avoid problems with file permissions; e.g., change it to “c:\nodejs"

|
|

Install and start DreamFace
---------------------------

When Node.js and MongoDB are properly installed, you can install DreamFace.

Create a directory (ex: "**\\dreamface**") in which an instance of the Cloud Application Platform will reside. Under the newly created directory, create a javascript file called **app.js** (note: you can give any other name to this file) that must contain the following code: ::

	require('dreamface').start();

This is the simplest way to initialize and start DreamFace from your platform. The ``require(...)`` instruction makes a reference and dependence with the "dreamface module". The ``start()`` function will start DFX on the default port (i.e 3000).

As with any Node.js application, you must provide an associated **package.json** file to your **app.js** which describes the application and its module dependencies: ::

	{
	  "name": "acme_cloud_app_platform",
	  "version": "1.0.0",
	  "description": "Acme Cloud App Platform",
	  "dependencies": {
		"dreamface": ">=1.0.56"
	  }
	}

Before running your Node application for the first time, the dependencies must be installed. To install the dependencies, issue the following command from the command line or system shell: ::

	<path of the new directory> npm install


All dependencies will be automatically downloaded and installed from the public repository (http://npmjs.org).


To launch and start DFX: ::

	<path of the new directory> node app.js


Upgrading DreamFace
-------------------

In the general case, the upgrade of DreamFace from a version to another is a simple modification of the dependence. Edit the **package.json** file and change the version number of the DreamFace dependency. Then issue the following command to update the installed module: ::

	<path of the new directory> npm install

All DreamFace files will be upgraded automatically.

Preparedness
~~~~~~~~~~~~

Before upgrading MongoDB always test your application in a staging
environment before deploying the upgrade to your production
environment.

Starting DreamFace with options
-------------------------------

But this string uses default settings of connection to a server and a database. In simple words, with this string, you connect to localhost on the 3000 port etc. This is not always what you need. The correct way is to require DFX, then initialize it with your own connection settings and then start DFX. Look at the example: ::

	var dreamface = require('dreamface');

	dreamface.init(null, null, {
	  'server_host': '188.232.12.147',
	  'server_port': 3002,
	  'mdbw_options' : { user: 'admin', pass: 'wRD9xJ97iTy', host: 'db.abc.com', port: 27018 },
	  'external_server_host': 'abc.com',
	  'external_server_port': 3002
	 });

	 dreamface.start();

Certainly, you should use your own host / IP and port values. Note that external_server_host and external_server_port are mandatory parameters, like the other ones in the example, and they are used to start DFX from remote computer. If they are not specified, their default values will be used from **dfx_settings.js** file.

In the ``init()`` function, the first null is an application identifier, and the second one is a host server.

By default, user and pass keys in ``mdbw_options`` parameter (database connection settings) are empty and can be omitted, but it depends on the settings of your Mongo server.

Default parameters are: ::

	'server_host': 'localhost',
	'server_port': 3000,
	'mdbw_options' : { user: '', pass: '', host: 'localhost', port: 27017 },
	'external_server_host': 'localhost',
	'external_server_port': 3000

You can omit any default parameter.

**So, if you need to change any parameter, you should use init() function; any amount of parameters passed is allowed; otherwise, you should not use this functions, if every parameter is default.**

Please note that it is better to use a domain name for external_server_host parameter rather than an IP address. This is the address where an application will be available, so it is better to specify a domain name.


Now the platform is ready to access and use.


Open the DFX console: http://localhost:3000/console in Chrome browser. At this time, the necessary database collections will be initialized automatically, if the database is empty. Enter with the following credentials: “**sys**” (login) and “**admin**” (password)  — during the first launch it is necessary to change the credentials (see the picture below). The initialization of the system happens automatically. MongoDB should be up and running.

.. image:: images/installation/DreamFace-Studio.png
	:width: 300px

The changing of the credentials is mandatory. After it there will be created the main user: admin (system administrator) with the access to the Studio Console.



Create a tenant, for example, “**demo**” (depending on the project you create). This will create collections and necessary records in the database.

.. image:: images/installation/create-a-tenant.png
	:width: 500px


**DFX system is multitenant. This means that the admin may create as many tenants as it is necessary.**

The tenant is not a user: this is a complete evironment. One server can contain several tenants which are executed simultaneously. The environment contains a repository with all its objects: widgets, data queries, applications, etc. DFX Studio is used to access these repositories. All the users, preferences, widgets, queries etc are described in the repository of a particular tenant.

Usually, every tenant has its own purpose: development of a project, different projects, demonstration, testing etc; and they can be named accordingly to their mission: "dev", "demo", "tests"...

During the creation of the tenant there is automatically created a developer with the administrative access to this tenant.


Now, click “Open Studio” and then press “Sign In”.

.. image:: images/installation/multitenant.png
	:width: 500px

This will open a page with the URL depending on the tenant identifier.

You can sign in with the following credentials: "admin" as the User ID and the password for the tenant which you have been specify while creating the tenant.

.. image:: images/installation/tenant-login.png
	:width: 300px

Now you can see the Studio Home Page.

.. image:: images/installation/home-page.png
	:width: 500px


Now that you've installed DreamFace and the DreamFace Compiler, it's time to build your first application :ref:`npmfirstapp-label`