
.. image:: ../../images/badges/badge_web.png
   :class: pull-right

Horizontalmenu
==============

.. image:: ../../images/icons/menu_horizontalmenu.png
    :width: 50px
    :height: 50px

A Horizontalmenu (sometimes referred to as Navigation Bar) is a menu that is displayed horizontally usually across the
top of a page. Each menu item can have an icon and any number of submenus. A Horizontalmenu can either have a static or
dynamic representation. The static menu is created in the Menu editor and the dynamic menu is defined in the script for
the view.

|

.. image:: ../../images/gcs/web/webgc-hzmenu.png

|

See it in Action
----------------

Try the Sample Buttons

.. toctree::
   :maxdepth: 1

   ../../gsguide/samples/sample-hzmenu

|

|

Reference
---------

The Horizontalmenu control properties can be set for the following property categories:

Main Properties
^^^^^^^^^^^^^^

.. toctree::
   :maxdepth: 1

   webgc-prop-main-id
   webgc-prop-main-template
   webgc-prop-main-name
   webgc-prop-main-display
   webgc-prop-main-menuitems

|

Styling Attributes
^^^^^^^^^^^^^^^^^^

Container Stying
''''''''''''''''

.. toctree::
   :maxdepth: 1

   webgc-prop-style-style
   webgc-prop-style-class
   webgc-prop-style-dynamic

Container Stying
''''''''''''''''

.. toctree::
   :maxdepth: 1

   webgc-prop-style-style
   webgc-prop-style-class
   webgc-prop-style-iconsize
   webgc-prop-style-style
   webgc-prop-style-class

Item Styling
''''''''''''
.. toctree::
   :maxdepth: 1

   webgc-prop-style-style
   webgc-prop-style-class
   webgc-prop-style-iconsize
   webgc-prop-style-style
   webgc-prop-style-class

|



+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Menu Items**         | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Static                 | Menu Editor       | Static means that the definition and contents of the menu/iconbar are static and once      |
|                        |                   | defined will remain the unchanged until they are manually changed again. The menu/iconbar  |
|                        |                   | can be defined by clicking on                                                              |
|                        |                   |        .. image:: ../../images/gcs/dfx-menu-edit-button.png                                |
|                        |                   | to bring the menu editor to assist in defining the menu/iconbar.                           |
|                        |                   |                                                                                            |
|                        |                   |                                                                                            |
|                        |                   |        .. image:: ../../images/gcs/dfx-help-menu-editor.png                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Dynamic                | NA                |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
|

.. _webgc-hzmenu-render-label:

Rendering
^^^^^^^^^

This is the rendering section.

|

.. _webgc-hzmenu-styling-label:

Styling Attributes
^^^^^^^^^^^^^^^^^^

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Styling Attributes** | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Style                  | CSS syles         | CSS style attribure(s) to use for this component, separated by semi-colons, for example:   |
|                        |                   | *color:red; background-color:lightgray*. By clicking on the **...** on the right hand side |
|                        |                   | of the field, a window opens up proposing to change attributes for **font**, **color**,    |
|                        |                   | **padding** and **margin** presented in a tree. When clicking on the arrow to the left of  |
|                        |                   | the attribute type, the user is guide by placeholder to enter the correct settings         |
|                        |                   |                                                                                            |
|                        |                   |        .. image:: ../../images/gcs/dfx-help-css-styles.png                                 |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Menu Style             | CSS class         | Name of CSS class to use for the component.                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Menu Icon Style        | CSS class         | Name of CSS class to use for the component.                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Item Style             | CSS class         | Name of CSS class to use for the component.                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Item Icon Style        | CSS class         | Name of CSS class to use for the component.                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Item Class             | CSS class         | Name of CSS class to use for the component.                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Dynamic Class          | CSS Class         | The Dynamic Class is a CSS class that will be added to the graphical control if an Angular |
|                        |                   | Expression is verified. It is rendered as a ng-class attribute.                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|


Events
^^^^^^

.. toctree::
   :maxdepth: 1

   webgc-events.rst


   |


**How to create a treemenu**

+-------------------------------------------------------------------------------------------------+-------------------------------------------------------+
| **Step Descriptions**                                                                           | Screen                                                |
+=================================================================================================+=======================================================+
| Drag and drop Treemenu GC to the working area, click on GC and then                             | .. figure:: ../../images/gcs/dfx-help-css-styles.png  |
| open Menu editor in popup by cliking Edit button in Property Panel.                             |     :width: 150px
| You’ll see default item: ‘Home’                                                                 |     :height: 75px                                     |
+-------------------------------------------------------------------------------------------------+-------------------------------------------------------+

|

Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.

|