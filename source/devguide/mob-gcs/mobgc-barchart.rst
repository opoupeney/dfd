.. image:: ../../images/badges/badge_mobile.png
   :class: pull-right


Barchart
=========

The pre-defined Charts graphical controls available in the Widget Editor are based on NDV3 library

|

.. image:: ../../images/gcs/mob/mobgc-barchart.png

|

The Barchart control properties can be set for the following property categories:

* :ref:`mobgc-barchart-main-label`
* :ref:`mobgc-barchart-options-label`
* :ref:`mobgc-barchart-styling-label`
* :ref:`mobgc-barchart-events-label`

|

.. _mobgc-barchart-main-label:

Main Properties
---------------

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Main Properties        | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Name                   | barChart#         | Name is a reference to the component's DOM element. It can be used to dynamically access   |
|                        |                   | and set component properties. DreamFace gives a default name of *barChart#* where #        |
|                        |                   | corresponds to the order in which it was created. If it's the second control created it    |
|                        |                   | will have a default Name of *barChart2*. Name is not required and can be removed if not    |
|                        |                   | needed.                                                                                    |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Binding                | $scope variable   | The data table can be bound to a value contained in a $scope variable.                     |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
|Title                   | Any text          | Title of the table, this can either be text in quotes or an                                |
|                        | Angular Expression| :ref:`angular-expression-label`.                                                           |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Display                | *true* or *false* | The value can be a literal **true** to display the component or **false** to hide it. This |
|                        | Angular Expression| value can also be the result of an :ref:`angular-expression-label` that returns a boolean  |
|                        |                   | value of the true or false, *true* meaning it will be visible, *false* meaning it will not |
|                        |                   | be displayed.                                                                              |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

.. _mobgc-barchart-options-label:

Options
-------

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Options**            | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| X-Axis Label           | Any text          | Title of the table, this can either be text in quotes or an :ref:`angular-expression-label`|
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Y-Axis Lable           | Any text          | Title of the table, this can either be text in quotes or an :ref:`angular-expression-label`|
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

.. _mobgc-barchart-styling-label:

Styling Attributes
------------------

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Styling Attributes** | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Size                   | size in dp        | Choose the size of the icon from the dropdown list by clicking on the drop arrow on the    |
|                        |                   | right of the size field.                                                                   |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Color                  | CSS color         | #hexcode for color| CSS colors are defined using a hexadecimal (HEX) notation              |
|                        | Predefined Cross- | (see :term:`Hexadecimal Colors`) or enter one of the Pre-defined cross browser colors.     |
|                        | Browser Colors    | `140 cross browser colors <http://www.w3schools.com/cssref/css_colornames.asp>`_           |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Class                  | CSS class         | Name of CSS class to use for the component.                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Dynamic Classes        | CSS Class         | The Dynamic Class is a CSS class that will be added to the graphical control if an Angular |
|                        |                   | Expression is verified. It is rendered as a ng-class attribute.                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Width                  | number of pixels  | Then number of pixels of the width of the Chart The defautl is 300px                       |
|                        |       n*px*       |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Height                 | number of pixels  | Then number of pixels of the height of the Chart The defautl is 250px                      |
|                        |       n*px*       |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

.. _mobgc-barchart-events-label:

.. include:: mobgc-props-events-state.rst

Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.

|
