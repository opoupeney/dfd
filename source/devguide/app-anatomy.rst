Anatomy of a DreamFace App
==========================

DreamFace applications are built using four main components :

|

Application Components
----------------------

|

====================   ==========================================================================================================================================
 **Component**         **Description**
====================   ==========================================================================================================================================
 **Navigation Menu**   Menu and Sub-Menus provide navigation through the application. Navigation starts with a Home Menu linked to the Home Page of the application. Menu Items are associated with Pages.
 **Pages**             Applications can have several Pages, each Page is composed of a number of Views arranged in a layout of rows and columns which makes up the user interface of the application.
 **Views**             Views (sometimes called Widgets) contain graphical controls like input fields, buttons and tables, arranged in a layout of rows and columns which makes up the User Interface of the View
 **API Services**      API Services provide access to the data by defining the different API Routes related to that service that access the data.
====================   ==========================================================================================================================================

|


Menu Navigation
---------------

The Navigation Menu provides a way to navigate through the application. By default the Navigation Menu starts with a Home Menu linked to the Home Page of the application.
The Navigation Menu is organized in a tree structure with Main Menu or top level either linked to a Page or containing sub-menu items. Each menu item is linked to a Page.
Each Page is a composition of Views, which in turn is a composition of Graphical Controls, Api Routes and scripts which define View behavior.

|

Page
----

A Page is a DreamFace component used to display one or more Views in a layout of rows and columns. A Page defines the user interface for
a part of the application, for example, a Page might display, update and delete Client data.


|

View
----

|

A View is a DreamFace component used to define the User Interface of an applciation or part of an application. Views are a composition of Graphical
Controls like input fields, buttons, tables that are provided as a list of pre-defined, ready to use Graphical Controls, available in the View Editor.
Graphical Controls are arranged in rows and columns in the View and are used to display and interact with data coming from the API Services and Routes.
Views are sometimes referred to as widgets. For a more information on available Graphical Controls see :ref:`gcontrols-label`

|

API Services
------------

An API Service is a DreamFace component that is used to consume public, private or internal APIs. An API Service is a DreamFace concept
used to make a logical grouping of API Routes. API Services are defined by Properties and API Routes. API Routes are components that define the access to back-end API Services.

For a more on API Services see :ref:`apiservices-label`

|
|
