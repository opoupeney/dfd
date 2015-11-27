Anatomy of a DreamFace App
==========================

DreamFace applications are cloud-native, multitenant applications consisting of Application Settings that define application behavior
and four main components that are the fundamental building blocks of a DreamFace app :

Application Components
^^^^^^^^^^^^^^^^^^^^^

====================   ==========================================================================================================================================
 **Component**         **Description**
====================   ==========================================================================================================================================
 **Navigation Menu**   Menu and Sub-Menus provide navigation through the application. Navigation starts with a Home Menu linked to the Home Page of the application. Menu Items are associated with Pages.
 **Pages**             Applications can have several Pages, each Page is composed of a number of Views arranged in a layout of rows and columns which makes up the user interface of the application.
 **Views**             Views (sometimes called Widgets) contain graphical controls like input fields, buttons and tables, arranged in a layout of rows and columns which makes up the User Interface of the View
 **API Services**      API Services group together related **API Routes** which define how to access public, private or internal back-end API data sources (usually REST services).
====================   ==========================================================================================================================================

.. image:: ../images/diagrams/dfd-app-anatomy.png

If we boil it down to just the basics we could say that a DreamFace application is a number of Views and Routes attached to an application.  Putting that in perspective,
applications also need navigation or application flow. In DreamFace the Navigation Menu manages the application flow defining which Page will be displayed when a menu
item is clicked. For desktop applications, Pages contain a composition of Views, organized in a layout of rows and columns. One View might have client information and
another may show sales for that client in a graph or a table view and a third view might show a map of where the client is located. This composition makes up the user
interface of the Page. The data that is used in the Page comes from the API Routes which are bound or linked to the View.

|

Navigation Menu
---------------

The Navigation Menu provides a way to navigate through the application. By default the Navigation Menu starts with a Home Menu linked to
the Home Page of the application. The Navigation Menu is organized in a tree structure with Main Menu or top level either linked to a Page
or containing sub-menu items. Each menu item is linked to a Page. Each Page is a composition of Views, which in turn is a composition of
Graphical Controls, Api Routes to interact with the data and scripts which define View behavior.

|

Page
----

A Page is a DreamFace component used to display one or more Views in a layout of rows and columns. A Page defines the user interface for
a part of the application, for example, a Page might display, update and delete Client data. Mobile applications do not use Pages as they
display the Views directly, one at a time.

|

View
----

A View is a DreamFace component used to define the User Interface of an application or part of an application. Views are a composition
of Graphical Controls like input fields, buttons, tables that are provided as a list of pre-defined, ready to use Graphical Controls,
available in the View Editor. Graphical Controls are arranged in rows and columns in the View and are used to display and interact with
data coming from the API Routes. Views are sometimes referred to as widgets.

For a more information on available pre-defined GraphicalControls available in the View Editor see :ref:`gcontrols-label`

|

API Routes
----------

An API Route is a DreamFace component that is used to consume public, private or internal APIs. An API Service is a DreamFace concept
used to make a logical grouping of API Routes. API Services are defined by Properties and API Routes. API Routes are components that
define the access to back-end API Services. DreamFace provides a number of ready to consume API Routes, for example in the API Service
Social Media you have predefined API Routes for facebook, twitter and other popular Social Media APIs.

For a more on API Services and API Routes see :ref:`apiservices-label`

|
|
