.. _getting-started-label:

Getting Started
===============

Get started building your first DreamFace app!

Follow the steps below to get up and running with your first DreamFace app. For a deeper dive, check out the :ref:`developer-guide-label`, which goes hands on into best practices and the most common use cases for developing with DreamFace.


.. toctree::
    :maxdepth: 1

    ../devguide/what-is-dreamface
    ../devguide/who-is-dfx-for
    ../devguide/prerequisites
    ../devguide/dfx-platform-architecture
    ../devguide/app-anatomy
    ../devguide/dev-process

|


Creating Your First App
-----------------------

The steps we'll take in guiding you to create your first app:

1. Setting up your cloud tenant
2. Exploring the Studio
3. Creating API Services
4. Creating Views
5. Creating Pages and Adding Views to a Page
6. Build and Compile the App
7. Deploy the App

1. Setting up your Cloud a tenant

Setting Up Your Cloud Tenant
Multitenancy refers to a principle in software architecture where a single instance of the software (i.e DreamFace) runs on a server, serving multiple client-organizations (tenants).
Multitenancy contrasts with multi-instance architectures where separate software instances (or hardware systems) operate on behalf of different client organizations. To simplify, many different clients-organizations can share the same mulitenant application and only one client-organization uses the software instance application.

You can use the multitenancy in DreamFace to suit your infrastructure needs. For example, a tenant can represent:

An environment (ex: dev, test, prod)
A business unit (ex: marketing, sales, finance)
An organization (ex: acme, durant)
An application domain (ex: demo, crm, portal)

For your first application we will use multitenancy to be an environment, for instance *dev*.

When you log in to the DreamFace Console the first time asAdmin you have no tenants.

Create a tenant called dev and give it a password.

Each tenant has access to a dedicated DreamFace Studio. All applications created in this tenant and all of the components that make
up the applications will be stored in a repository linked to this tenant and will be completely isolin


Exploring the Studio

Creating API Services

Creating Views

Creating Pages and Adding Views to a Page

Build and Compile the App

Deploying the App



Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.