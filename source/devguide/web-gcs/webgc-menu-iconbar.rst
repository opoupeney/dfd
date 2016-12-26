
.. image:: ../../images/badges/badge_web.png
   :class: pull-right

Iconbar
=======

 .. image:: ../../images/icons/menu_iconbar.png
    :width: 50px
    :height: 50px

An iconbar is a menu of icons. It has a top level menu that shows icons which is is a menu item. Menu items can have sub
menu items. The iconbar menu is defined in the Menu Editor.

|

.. image:: ../../images/gcs/web/webgc-iconbar.png

and with sample icons:

.. image:: ../../images/gcs/web/webgc-iconbar-example.png

|

See it in Action
----------------

Try the Sample Buttons

.. toctree::
   :maxdepth: 1

   ../../gsguide/samples/sample-iconbar

    |

|

Reference
---------

The Icon control properties can be set for the following property categories:

* :ref:`webgc-iconbar-main-label`
* :ref:`webgc-iconbar-render-label`
* :ref:`webgc-iconbar-styling-label`
* :ref:`webgc-iconbar-events-label`


|

Main Properties
^^^^^^^^^^^^^^

.. toctree::
   :maxdepth: 1

   webgc-prop-main-id
   webgc-prop-main-template
   webgc-prop-main-name
   webgc-prop-main-label
   webgc-prop-main-icon
   webgc-prop-main-display
   webgc-prop-main-disabled

|

Styling Attributes
^^^^^^^^^^^^^^^^^^

.. toctree::
   :maxdepth: 1

   webgc-prop-style-style
   webgc-prop-style-class
   webgc-prop-style-dynamic

|


+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Main Properties**    | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Name                   | iconBar#          | Name is a reference to the component's DOM element. It can be used to dynamically access   |
|                        |                   | and set component properties. DreamFace gives a default name of *icoBar#* where #          |
|                        |                   | corresponds to the order in which the control was created. The second iconbar control      |
|                        |                   | created it will have a default Name of *icoBar2*. Name is not required and can be removed  |
|                        |                   | if not needed.                                                                             |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Display                | *true* or *false* | The value can either be a literal *true* to display the field or *false* to hide it. It can|
|                        | angular expression| also be a angular expression that evaulates to *true* or *false*, for example,             |
|                        |                   |                                                                                            |
|                        |                   | 5 > 2 would evaluate to *true* and 5 < 2 would evaluate to false                           |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
|

.. _webgc-iconbar-render-label:

Rendering
^^^^^^^^^

This is the rendering section.

|

.. _webgc-iconbar-styling-label:

Styling Attributes
^^^^^^^^^^^^^^^^^^

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Styling Attributes** | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| xxxxxxx                | CSS class         | Name of CSS class to use for the component.                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Style                  | CSS syles         | CSS style attribure(s) to use for this component, separated by semi-colons, for example:   |
|                        |                   | *color:red; background-color:lightgray*. By clicking on the **...** on the right hand side |
|                        |                   | of the field, a window opens up proposing to change attributes for **font**, **color**,    |
|                        |                   | **padding** and **margin** presented in a tree. When clicking on the arrow to the left of  |
|                        |                   | the attribute type, the user is guide by placeholder to enter the correct settings         |
|                        |                   |                                                                                            |
|                        |                   |        .. image:: ../../images/gcs/dfx-icon-css.png                                        |
+------------------------+-------------------+-------------------------------------------------------------------------------------------+|
| Classes                | CSS class         | Name of CSS class to use for the component.                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Dynamic Classes        | CSS Class         | The Dynamic Class is a CSS class that will be added to the graphical control if an Angular |
|                        |                   | Expression is verified. It is rendered as a ng-class attribute.                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

Events
^^^^^^

.. toctree::
   :maxdepth: 1

   webgc-events.rst

Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.

|
