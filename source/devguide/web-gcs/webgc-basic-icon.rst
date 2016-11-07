.. image:: ../../images/badges/badge_web.png
   :class: pull-right

Icon
====

.. image:: ../../images/icons/basic_icon.png
    :width: 50px
    :height: 50px

An icon is a graphical image that conveys a message, for example an image of a telephone might indicate that the View is
about telephone numbers, a house might mean to fill in your home address in a form.

|

.. image:: ../../images/gcs/web/webgc-icon.png

|

Features
--------
* Full selection of SVG Icons with Categories Menu
* Full selection of Font Awesome Icons
* Help feature allows selection / search for icon

|

See it in Action
----------------

Try the Sample Iconss

.. toctree::
   :maxdepth: 1

   ../../gsguide/samples/sample-icons

|

Reference
---------

The Icon control properties can be set for the following property categories:

* :ref:`webgc-icon-main-label`
* :ref:`webgc-icon-render-label`
* :ref:`webgc-icon-styling-label`
* :ref:`webgc-icon-events-label`

|

.. _webgc-icon-main-label:


Main Properties
^^^^^^^^^^^^^^^

|

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Main Properties**    | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Name                   | icoIcon#          | Name is a reference to the component's DOM element. It can be used to dynamically access   |
|                        |                   | and set component properties. DreamFace gives a default name of *icoIcon#* where #         |
|                        |                   | corresponds to the order in which the control was created. If it's the second icon control |
|                        |                   | created it will have a default Name of *icoIcon2*. Name is not required and can be removed |
|                        |                   | if not needed.                                                                             |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| label                  | Any text          | This is the text that will appear under the icon, for example the fa-home icon could have  |
|                        |                   | the label Home as DreamFace uses as the default for this component.                        |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| icon                   | favicon           | Click on the **...** to the right of the field to select one of the favicons from the list.|
|                        |                   |                                                                                            |
|                        |                   |        .. image:: ../../images/gcs/dfx-icons.png                                           |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Display                | *true* or *false* | The value can either be a literal *true* to display the field or *false* to hide it, or it |
|                        | angular expression| be a angular expression that evaulates to *true* or *false*, for example,                  |
|                        |                   |                                                                                            |
|                        |                   | 5 > 2 would evaluate to *true* and 5 < 2 would evaluate to false                           |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Disabled               | *true* or *false* | *true* to disable the field or *false* to make it active or it be a angular expression that|
|                        | angular expression| evaulates to *true* or *false*, for example,                                               |
|                        |                   |                                                                                            |
|                        |                   | 5 > 2 would evaluate to *true* and 5 < 2 would evaluate to false                           |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+


.. _webgc-icon-render-label:

Rendering
^^^^^^^^^

This is the rendering section.


.. _webgc-icon-styling-label:


.. include:: webgc-styling.rst

|

.. _webgc-icon-events-label:

.. include:: webgc-events.rst

Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.

|