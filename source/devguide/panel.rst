Panel
=====

.. image:: ../images/icons/icon_web.png
   :class: pull-right

|

Description
^^^^^^^^^^^

The image graphical control is used to display images. An image is specified using a url. Images can be from external or internal sources. Internal sources can be imported using resources to add the image as a resource.

|

Properties
^^^^^^^^^^

**Main Properties**

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Main Properties        | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Name                   | imgImage#         | Name is a reference to the component's DOM element. It can be used to dynamically access   |
|                        |                   | and set component properties. DreamFace gives a default name of *imgImage#* where #        |
|                        |                   | corresponds to the order in which it was created. If it's the second accordion created it  |
|                        |                   | will have a default Name of *imgImage2*. Name is not required and can be removed if        |
|                        |                   | not needed.                                                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| External URL           | Any text          | Specifies the URL of an image on another website. The URL can be an expression.            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Local URL              | associated url    | Specifies the URL of an image (imported in resources).  The url can be an expression.      |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Tooltip                | Any text          | Tip to help the user. It will be displayed when mouse passes over this control. Tooltip    |
|                        |                   | text can also be an expression.                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Tooltip Position       | *top*             | Position where tooltip will be displayed when mouse passes over.                           |
|                        | *left*            |                                                                                            |
|                        | *bottom*          |                                                                                            |
|                        | *right*           |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+



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
| Classes                | CSS class         | Name of CSS class to use for the component.                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Dynamic Classes        | CSS Class         | The Dynamic Class is a CSS class that will be added to the graphical control if an Angular |
|                        |                   | Expression is verified. It is rendered as a ng-class attribute.                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Events**             | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| On Click               | function name     | Enter the name of the function that will be executed when the user clicks on the HTML      |
|                        |                   | control. The function should be defined in the controller in the script tab of the View    |
|                        |                   | Editor. Clicking on the ... opens a window to to select a function defined in the          |
|                        |                   | Controller.                                                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+


|
|
