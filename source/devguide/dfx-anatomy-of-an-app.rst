.. _dfx-app-anatomy-label:

Anatomy of a DreamFace Application
==================================

A DreamFace application consists of an :ref:`application-configuration-label` and a set of :ref:`application-components-label`.


.. figure:: ../images/diagrams/DFX-App-Anatomy-V3.png
   :width: 700px

   *Figure - DreamFace Applications use Templates to define the look and feel of a Page. Pages are a composition of Views. Views
   consume API Service Objects, a logical group of API Services, to expose data. API Services use API Sources to define their
   access to APIs.*

|

A DreamFace Application is defined by its Application Configuration and the Application Components that make up the application.

.. _application-configuration-label:

Application Configuration
-------------------------

The main Configuration Settings to get started are listed below:




======================  ==================================================================================================================================================================================
 **Setting**            **Description**
======================  ==================================================================================================================================================================================
 **API Sources**        An API Source is a reusable definition that defines how to access the backend API, including which authentication protocol and developer credentials are needed to access it.
 **Resources**          External resources such as javascript files, css files and other assets like images or icons which can be added to extend the DreamFace Platform and are available throughout the application.
 **Users**              Templates define the layout and look and feel of a Page (header, footer, left nav, right nav, body, etc.).
======================  ==================================================================================================================================================================================


See the Refenence Guide section :ref:`dfx-studio-explorer-label` for a complete presentation of the Studio Explorer or
visit :ref:`app-config-label` to learn about other settings in the Application Configuration.

|

.. _application-components-label:

Application Components
----------------------

* DreamFace applications use Templates to define the look and feel of a Page.
* Pages are a composition of Views that consume and are bound to API Services which are grouped together in API Service Objects.
* API Services use API Sources to define API access.

|

The different components that make up a DreamFace application are :

==============================  ===================================================================================================================================================================================
 **Setting**                     **Description**
==============================  ===================================================================================================================================================================================
 **Templates**                  Templates define the layout and look and feel of a Page (header, footer, left nav, right nav, body, etc.).
 **Pages**                      Applications can have several Pages, each Page is composed of a number of Views arranged in a layout of rows and columns to form the :term:`UI` of the Page.
 **Views**                      Views (sometimes called Widgets) are graphical views which contain graphical controls ike input fields, buttons and tables arranged in a layout of rows and columns. Views are reusable across Pages. Views contains “cards” (a notion of multi-layering, :term:`SPA`) allowing some very complex interface representations to be built easier.
 **API Service Objects**        API Service Objects provide access to the data by defining the different API Services and their Routes. These are are endpoints that reference virtually any API end point that needs to be called in the application. API Services are organized under the notion of an “API Service Object” whichh allows them to be better classified and managed. They connect to the backend using “API Sources” (handlers that contains the type of the backend to call, the URL and the security credentials).
==============================  ===================================================================================================================================================================================

|

Page Templates
^^^^^^^^^^^^^^

A Page Template is a developer/designer concept that defines the "look and feel" or model to be used for each page of the
application.

A “Page Template” is defined graphically using the DreamFace *Page Editor*.

.. image:: ../images/devguide/dfx-page-editor.png

The *Page Editor* can be used to build

* a Single View Page Template containing
* a Single View Page Template with a Left Navigation and / or Right Navigation
* Multiple View Page Template with a bottom navigation and a header

The Header, the Body and the Left and Right navigation panels can be populated with Views. The Page Template can have
“locked areas” where developers using the Template are not alloz alter these areas) and “unlocked areas” (developers can drop their
views in theses areas while composing application pages). This mechanism ensures consistency in developing User Interfaces
where only a few Templates may be needed to develop an entire application.

|

Pages
^^^^^

A Page is a DreamFace component used to display one or more Views in a layout of rows and columns. A Page defines the user interface for
a part of the application, for example, a Page might display, update and delete Client data. Mobile applications do not use Pages as they
display the Views directly, one at a time.


Pages are graphical elements that are composed of:

* One Page Template
* One or many Views

Pages are the graphical compositions through which a user interacts with the application.

.. image:: ../images/devguide/dfx-page-editor.png


Pages have their own controller for:

* Page wide actions
* Page wide scope (variables, functions, etc.)
* A specific view can refer to “parent scope” (i.e. the instance of the page in which it is rendered)

Pages uses Templates in order to respect a specific Look & Feel.

|

Views
^^^^

Views are the core component of the User Interface in DreamFace. Views are functional graphical areas, with an embedded
logic (via the controller) as well as a REST based invocation interface. Views are deployed as :term:`Angular modules`.
Views are usually assembled in Pages and communicate with each other via a natively supported :term:`pub/sub mechanism.

Views are a composition of Graphical Controls like input fields, buttons, tables that are arranged in rows and columns
in the View and are used to display and interact with data being exchanged with API Services. Outside of DreamFace, Views
are sometimes referred to as widgets.

For a more information on available pre-defined GraphicalControls available in the View Editor for use in Views see :ref:`gcontrols-label`


.. image:: ../images/devguide/dfx-view-ineditor.png

When deployed in a page, views can:

* communicate with each other via a pub/sub mechanism. This mechanism will evolve in a near future to become the foundation
of the “View Interface”. An easy programming model to allow the implementation of “onBusinessEvent do…” will be implemented.

The sum of all events handled by the View or Emitted by the View will become the “View Interface” allowing an easy and
graphical wiring between Views in order to produce a more granular concerted experience.

* Access a higher level context such as the ones for the host page or the applicaton


** Cards**

Cards are a very interesting concept that was added in DreamFace v3.0. The idea of Cards stemmed from the need to produce
MicroServices where a concerted set of Views are needed as part of the “UI module” in a “Single Page UI Design” :term:`SPA`.
For example, A Micro Service can be made from a View that shows the Customer list in a Table, clicking on a customer to
edit the properties in a form like fashion, along with a variety of Dialogs to confirm actions. In order to easily implement
such an interaction, Cards can be used in order to provide the variety of “layers” needed for such an interaction, where
a context links them together and where a variety of look & feel can be needed “Cards” implements the facility to allow
the development of “multiple views within the same view”. They allow the implementation of a “depth” or a “layering model”
to the view where very complex representations can be easily produce.

All Cards share the same “controller” allowing them to share information easily without the need of a pub/sub mechanism.
Cards can be invoked in a variety of ways in order to be shown as a “sliding view: left/right/bottom” or a Dialog Box or
even to become the default Card to occupy the whole real estate of a view.
* Example of Card ?? <<Show graphical Examples >>
* Example of View ?? <<show code that invokes it>>



API Integration
---------------

DreamFace applications consume API services exclusively. All interactions with backend systems for data access are modeled
as API calls, using the REST standard as a way to interact and standardize the consumption of services. DreamFace introduces
many new concepts to ease the adaptation and the consumption of API’s for the purpose of building the User Interface.


API Source
^^^^^^^^^^

“API Sources” are the construct to define a “backend API source” to be used later on to define services. An “API Source”
is the equivalent concept to a DataSource in the DataBase metaphor. An API Source defines:

* Type of the API endpoint (REST, XML,WebService, DataBase, etc..)
* URL/Address of the endpoint
* Security Type and credentials

DreamFace provides an added value to some of the providers in order to ease the interaction effort:

* REST to XML mapping
* DataBase consumption and mapping to REST
* Introspection of some of the backends (such as StrongLoop , Swagger, etc.) in order to allow an interactive consumption of such backend services
* High Value add services: List of “specific usable providers” such as SalesForce API, NetSuite API, Weather.com, News API, Google API, etc. These providers’ services will be ready for consumption “out of the box”. DreamFace engineers and/or user community will be adding to this list in order to provide an exponential value to the whole user community


API Service Object
^^^^^^^^^^^^^^^^^^

API Service Object is a concept to gather “business related services” in a single object construct and this, regardless
if the Services endpoint are provided from the same source or not.An example, an “API Service Obejct” called “News” can have services (aka methods) such as “getCNNNews” or “getYahooNews” as well as get “getAllNews”, irrespective if the news are using the same API Source or not. This association via the Service Ibejct will be enriched in the future to allow a “common behavior” at the Object level such as accessibility rules, caching rules, filtering rules, etc.
<<schema to depict the concept of API Service Ibject>>

API Services
^^^^^^^^^^^^

An API Service is a concept that maps to a specific end point API. An API Service is one interaction with the backend.
The basic concepts to retain on API Services in DreamFace are
-	An API Service Object is made of one or more API Servcie(s)
-	An API Service
o	Maps to an API URL. This URL can be manually entered or introspected if the backend source allows it
o	Uses an API Source to determine the nature of the backend as well as the security credentials to access it
o	Always take a JSON in and produces a JSON out. The notion of these in/out payload makes the API Service Interface. Future releases of DreamFace will extend on the notion of these interfaces in order to build a “Business Object Repository” that maps the interfaces to reusable BO constructs to be used between the backend and front end sides of an application
o	PreHandler/PostHandler/Application Exception Handler: These NodeJS modules of codes will allow the API Service that is declared in DreamFace to have an intelligent behavior that overloads the API call to the backend.  Through these mechanisms, once can filter the API call to the backend, overload it, merge API invocations, aggregate API calls, etc.

API Services can be consumed by any REST client (postman for example). DreamFace adds an embedded Oauth2 security to these
API Services making a non-secured backend automatically secured.

An API Route is a DreamFace component that is used to consume public, private or internal APIs. An API Service is a DreamFace concept
used to make a logical grouping of API Routes. API Services are defined by Properties and API Routes. API Routes are components that
define the access to back-end API Services. DreamFace provides a number of ready to consume API Routes, for example in the API Service
Social Media you have predefined API Routes for facebook, twitter and other popular Social Media APIs.

For a more on API Services and API Routes see :ref:`apiservices-label`

|

Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.

