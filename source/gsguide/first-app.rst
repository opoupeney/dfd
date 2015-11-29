Creating My First App
=====================

* Creating a tenant
* Exploring the Studio
* Creating API Services
* Creating Views
* Creating Pages and Adding Views to a Page
* Build and Compile the App
* Deploy the App

Creating Your First App
-----------------------

Follow the steps below to create your first app:

1. Setting up your cloud tenant
2. Exploring the Studio
3. Creating API Services
4. Creating Views
5. Creating Pages and Adding Views to a Page
6. Build and Compile the App
7. Deploy the App

|

**1. Setting up your Cloud a tenant**

Multitenancy refers to a principle in software architecture where a single instance of the software (i.e DreamFace) runs on a server,
serving multiple client-organizations (tenants). Multitenancy contrasts with multi-instance architectures where separate software
instances (or hardware systems) operate on behalf of different client organizations. To simplify, many different clients-organizations
can share the same mulitenant application and only one client-organization uses the software instance application.

You can use the multitenancy in DreamFace to suit your infrastructure needs. For example, a tenant can represent:

An environment (ex: dev, test, prod)
A business unit (ex: marketing, sales, finance)
An organization (ex: acme, durant)
An application domain (ex: demo, crm, portal)

For your first application we will use multitenancy to be an environment, for instance *dev*.

When you log in to the DreamFace Console for the first time as Admin you have no tenants.

Create a tenant called dev and give it a password.

Each tenant has access to a dedicated DreamFace Studio. All applications created in this tenant and all of the components that make
up the applications will be stored in a repository linked to this tenant and will be completely isolated.


**2. Exploring the Studio**

**3. Creating API Services**

**4. Creating Views**

**5. Creating Pages and Adding Views to a Page**

**6. Build and Compile the App**

**7. Deploying the App**


Getting Starting DreamFace Tutorial Series
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Welcome to the series on Getting Started with DreamFace for Web Applications.

This course will cover all the fundamentals that you need to get started building business applications for the web with DreamFace. It is designed to teach you everything you need to know about how to use DreamFace as well as best practices on how build great applications.

Each lesson builds on the previous one. To get the most from this course, view the tutorials in order.

.. _gettingstarted-label:

Getting Started Tutorials Menu
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. toctree::
:maxdepth: 1

        first_app
        cloud-tenant
        development-process
        application-architecture
        creating-widgets
        widget-editor
        connecting-data
        adding-resources
        application-personalization
        deploying
        cloud-database
        cloudapp-settings
        registering-theme
        registering-url

|
|