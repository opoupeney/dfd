.. image:: ../../images/badges/badge_web.png
   :class: pull-right

Richtext
========

.. image:: ../../images/icons/input_richtext.png
    :width: 50px
    :height: 50px


A richtext control provides a number of properties you can be used to apply formatting to any portion of text within the
control in a view at runtime of your application.

To change the formatting of text, selecct the part of the text to format and assign the desired formatting.
Using formatting, you can make text bold or italic, change the color, font and many other styles.

|

.. image:: ../../images/gcs/web/webgc-richtext.png

|

See it in Action
----------------

Try the Sample Richtext

.. toctree::
   :maxdepth: 1

   ../../gsguide/samples/sample-richtext

    |

|

Reference
---------


The Richtext control properties can be set for the following property categories:

* :ref:`webgc-richtext-main-label`
* :ref:`webgc-richtext-render-label`
* :ref:`webgc-richtext-styling-label`
* :ref:`webgc-richtext-layout-label`
* :ref:`webgc-richtext-events-label`


.. _webgc-richtext-main-label:

Main Properties
^^^^^^^^^^^^^^

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
|Title                   | Any text          | Title text or expression defines title of the panel.                                       |
|                        | Angular Expression|                                                                                            |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Title Visible          | Boolean value     | Title visible can either be set directly using *true* or *false* values or can be the      |
|                        | Angular Expression| result of an angular expression that returns a boolean value of the true or false, $true*  |
|                        |                   | meaning the title will be visible, *false* meaning title will not be displayed.            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Whiteframe             | number in dp units| Defines the border of the panel in :term:`dp` units, the higher the value of the dp the    |
|                        |                   | more shadow depth the panel will have which helps the user with the perception of which    |
|                        |                   | object is above the other.                                                                 |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Display                | Any text          | Tip to help the user. It will be displayed when mouse passes over this control. Tooltip    |
|                        |                   | text can also be an expression.                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Repeatable**         | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
|Repeat for all $item in | Any text          | Title text or expression defines title of the panel.                                       |
|                        | Angular Expression|                                                                                            |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
|

.. _webgc-richtext-render-label:

Rendering
^^^^^^^^^

This is the rendering section.

|

.. _webgc-richtext-styling-label:

.. include:: webgc-styling.rst

|

.. _webgc-richtext-layout-label:

Layout Properties
^^^^^^^^^^^^^^^^^


+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Layout Properties**  | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| row #                  | number            | Number of a row in the panel                                                               |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| col #                  | number            | Number of a column in the panel                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| width                  | number in pixels  | The width of the column in pixels. Default value is 100px.                                 |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| layout direction       | number            |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Hor. alignment         | number            | This value is chosen from a drop down list. Default value is *start*.                      |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Ver. alignment         | number            | This value is chosen from a drop down list. Default value is *start*.                      |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Style                  | CSS styles        | CSS style attribure(s) to use for this component, separated by semi-colons, for example:   |
|                        |                   | *color:red; background-color:lightgray*.                                                   |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Classes                | CSS class         | Name of CSS class to use for the component.                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Dynamic Classes        | CSS Class         | The Dynamic Class is a CSS class that will be added to the graphical control if an Angular |
|                        |                   | Expression is verified. It is rendered as a ng-class attribute.                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|


Events
^^^^^^

.. toctree::
   :maxdepth: 1

   webgc-events-onchange.rst

Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.

|