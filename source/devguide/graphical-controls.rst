.. _gcontrols-label:

Graphical Controls
------------------

DreamFace is designed to help you build both web and cross-platform mobile applications.

When deciding which kind of interface you want for your applications, you have a few different options:

* **Web UI** - built to run desktop browser-based applications. Because it is :term:`responsive` it can also be used from mobile devices in a mobile browser.
* **Mobile UI** - built specifically for mobile apps and can generate a zip file for Phonegap Build to create a cross-platform version for different mobile operating systems.

Building web applications requires different graphical controls than mobile applications due to the screen size and need
to present information differently. For this reason, DreamFace includes two different View editors, one for building the user
interface of web applications and one for building the UI of mobile apps. Each editor contains its own set of pre-defined
graphical controls. Pre-defined graphical controls are :term:`UI` components that are ready to use in Views like input fields,
buttons, tables, charts and panels. In the visual View Editor you drag and drop these controls onto a panel and set properties
for the specific functionality required by your application.

The same API Services and their corresponding API Routes can be used by both web and mobile applications.

For a detailed explanation of each View Editor's pre-defined graphical controls in the sections below.

|
|

.. _webgcs-label:

Web Application Graphical Controls
----------------------------------

DreamFace uses Angular Material to define the look and feel of web application graphical controls.

When creating your application you specify that the application is a web application. Web applications will automatically
have access to the View Editor containing the pre-defined graphical controls for building web apps. They are divided
into three categories:

* **Default** - Default Graphical Controls are usually associated with only one input field and value.
* **Chart** - Charts are complex graphical controls which can be easily created and configured with drag-drop and parameter settings which determine their behavior and how they visualize data
* **Layout** - Layout controls define the composition of the View component for presenting information in rows and columns


Default
^^^^^^^

Simple graphical controls are associated with one input field. Below is a description of each Default graphcical control
available in the View Editor for building desktop browser-based applciations :

.. toctree::
   :maxdepth: 1

   statictext
   button
   icon
   image
   input
   datepicker
   select
   checkbox
   slider
   switch
   knob
   html
   chips
   radio
   rating
   datatable

|

Chart
^^^^^

Charts help to put information in context. Below is a description of each pre-defined chart available in the View Editor:

.. toctree::
   :maxdepth: 1

   barchart
   piechart
   linechart

|

Layout
^^^^^^

Layout is a special graphical control that defines how the View Component will be organized in rows and columns. Below is
a description the panel pre-defined graphcical control that defines the layout for our View:

.. toctree::
   :maxdepth: 1

   panel

|
|

