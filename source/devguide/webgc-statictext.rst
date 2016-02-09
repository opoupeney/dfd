Statictext
===========

.. image:: ../images/icons/icon_web.png
   :class: pull-right

Statictext controls display text that does not require user input. They often serve as labels for other controls or to indentify
areas of the View. They can also be used to display icons that add context to the user interface.

|

.. image:: ../images/gcs/dfx-statictext-designtime.png

|

Properties
^^^^^^^^^^

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Main Properties**    | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Name                   | txtText1#         | Name is a reference to the component's DOM element. It can be used to dynamically access   |
|                        |                   | and set component properties. DreamFace gives a default name of *txtText#* where #         |
|                        |                   | corresponds to the order in which the control was created. The second statictext created   |
|                        |                   | will have a default Name of *txtText12*. Name is not required and can be removed if not    |
|                        |                   | needed.                                                                                    |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Text                   | Any text          | Text that will be displayed in the field. It should be in quotes, otherwise it will be     |
|                        |  *expression*     | treated as a variable.                                                                     |
|                        |                   |                                                                                            |
|                        |                   | **Text can also be an expression** which will be evaluated at runtime.                     |
|                        |                   |                                                                                            |
|                        |                   | See more about how to define :ref:`expressions-label` here.                                |
|                        |                   |                                                                                            |
|                        |                   | *Note* - Text needs to be in quotes otherwise it will be treated as a variable. If your    |
|                        |                   | label doesn't appear in Preview mode, make sure the text is in quotes. For words that      |
|                        |                   | contain an apostrophe, use double quotes. For example "It's a button" would evaluate to:   |
|                        |                   |                                                                                            |
|                        |                   | *It's a button* at runtime (in Preview Mode or when testing the application).              |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Display                | *true* or *false* | The value can either be a literal *true* to display the field or *false* to hide it, or it |
|                        | angular expression| be a angular expression that evaulates to *true* or *false*, for example,                  |
|                        |                   |                                                                                            |
|                        |                   | 5 > 2 would evaluate to *true* and 5 < 2 would evaluate to false                           |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Styling Attributes** | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Style                  | CSS syles         | CSS style attribure(s) to use for this component, separated by semi-colons, for example:   |
|                        |                   | *color:red; background-color:lightgray*.                                                   |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Classes                | CSS class         | Name of CSS class to use for the component.                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Dynamic Classes        | CSS Class         | The Dynamic Class is a CSS class that will be added to the graphical control if an Angular |
|                        |                   | Expression is verified. It is rendered as a ng-class attribute.                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Tooltip Properties** | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Tooltip Text           |  Any text         | Tip to help the user know what to do. It will be displayed when mouse passes over this     |
|                        |                   | control. The Tooltip Text can also be an expression.                                       |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Tooltip Direction      | Left, Top,        | A radio button is provided with the values Left, Top, Bottom or Right corresponding to the |
|                        | Bottom, Right     | position where the tooltip will be displayed relative to the text.                         |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Events**             | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| On Click               | function name     | Enter the name of the function that will be executed when the user clicks on the Static    |
|                        |                   | control. The function should be defined in the controller in the script tab of the View    |
|                        |                   | Editor. Clicking on the ... opens a window to to select a function defined in the          |
|                        |                   | Controller.                                                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Add Directive**      | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
|  Extended Directives   | function name     | This allows you to add extended directives to customize the default Statictext and add     |
|                        |                   | functionality. When you click on *Add Directive*                                           |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+


|
|
