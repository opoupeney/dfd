Architecture of the DreamFace Platform
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ../images/diagrams/dfd-gs-platform.png


The DreamFace Platform that you use to develop applications is a cloud-based, multitenant development platform built on :term:`MEAN Stack` technologies.
It is composed of three main applications called editions:

* **DreamFace Developer Edition** is used to create applications and includes the DreamFace Studio where most of the magic happens
* **DreamFace Compiler Edition** is used to compile and manage different builds of your application
* **DreamFace Deployment Edition** is used to host and run deployed apps

|

DreamFace Developer Edition
---------------------------

The DreamFace Developer Edition provides the develpment platform for creating DreamFace applications.

The DreamFace Developer Edition is a cloud-native, multitenant development platform. The main component of this edition is the DreamFace Studio which contains all of the components for building DreamFace applcations. In the DreamFace Studio
there are View Editors for creating desktop and mobile applications using pre-defined graphical controls. DreamFace is open and extensible so you can also
add your own custom graphical controls. The DreamFace View Editors have a preview capability for the iterative process of creating and testing Views.
When adding applcation logic DreamFace provides a script editor where you write your script in javascript and Angular.

|

DreamFace Compiler Edition
--------------------------

The DreamFace Compiler Edition compiles DreamFace applications and manages the builds that are created during the compilation.

**How the compiler works**

From the Cloud Platform menu under System Configuration & Setting is the Deployment option. When you click on it,
the Application Builds view is displayed.  On the bottom half of the view is the Build History list indicating Build
Version, Build Description, Date of Build, Status of Build (success, pending, failed) and Actions that can be taken
(Deploy, Download the zip if it is a Mobile application and Delete Build). The list is displayed with the most
recent build on top and the oldest build on the bottom.

Before you start your build you can set the Application Version to the version you wish to create. When you click on
Build Now the next Build Version Number will be based on the application version number and the build number, so for
Application Version: 1.0 and Build Number 3 will give a Build Version of 1.03.

To create a build, the DreamFace Studio sends an asynchronous request to the DreamFace Compiler to compile your specific
application. The asynchronous call means you can continue developing or watch the progress of the compilation until it
finishes.

Each component is compiled independently. While the compiler is working it will set the status to 'pending'. If you click
on the Pending status button an view is opened to show progress information about the build including percentage completion
the and the name of View currently being compiled.

When compilation is complete, the compiler sends back a status of 'success' or 'failed'. A status of 'success' indicates that the compilation is
complete and every component was compiled successfully. When compilation is successful, the compiler sends back a zip file and a log file
containing stack trace information.

If the compiler encounters errors it won’t stop the compilation. Each component will go through compilation. When finished, if status is 'failed',
no zip file is returned and if you click on the log file a View will open up providing more information and indicate the View(s) that failed
compilation. where errors occurred thus helping you to debug the application by identifying Views that contain errors. For example, it might indicate “View X and Y compiled successfully View Z failed to
compile. The developer can look at the stack trace in the log file to see where the error(s) occurred and fix the problem.

In an application with 10 View components, if 2 fail compilation, the log file will indicate it, so instead of compiling and failing on one component at a time, the DreamFace Compiler takes
the approach of identifying all problem components so you can save time in debugging and fixing your application.

By default the DreamFace Studio will reside on port 3000 and the Dreamface Compiler on port 3030. The compiler can also be
set to run on another port or server by setting an option in the Application Configuration and Settings.

|

DreamFace Deployment Edition
----------------------------

Successful Builds can be deployed. From the list of successful builds you can click on the small cloud icon to deploy the build.

The DreamFace Deployment Edition is a streamlined, lightweight runtime version of the DreamFace Developer Edition.
It is built for speed of execution and efficiency.

Deployed Builds are shown in a list at the top of the Deployment View. The list of Deployed Builds includes
Application Version, Build Number and Build Date.

|
|