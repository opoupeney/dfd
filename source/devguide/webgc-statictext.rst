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
| Text                   | Any text          | Any text that will be displayed in the field. It should be in quotes, otherwise it will be |
|                        |  *expression*     | treated as a variable.                                                                     |
|                        |                   |                                                                                            |
|                        |                   | **Text can also be an angular expression** which will be evaluated at runtime.             |
|                        |                   |                                                                                            |
|                        |                   | See more about how to define :ref:`angular-expression-label` here.                         |
|                        |                   |                                                                                            |
|                        |                   | On the right hand side of the field you will see **...** indicating that help in defining  |
|                        |                   | expression is available. Click on the *...** and a Expression View will be displayed,      |
|                        |                   | incidicating defined scope variables and functions.                                        |
|                        |                   |                                                                                            |
|                        |                   | **Note** - If your label doesn't appear in Preview mode, make sure the text is in quotes.  |
|                        |                   | If you have an angular expression that does not appear in Preview mode it means that their |
|                        |                   | most likely an error in your angular expression. Take a look at the sample angular         |
|                        |                   | expressions in the Samples Gallery. If your expression contains an apostrophe, use double  |
|                        |                   | quotes. For example "It's a button" would evaluate to: *It's a button* at runtime or in    |
|                        |                   | in Preview Mode when testing the View.                                                     |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Display                | *true* or *false* | The value can either be a literal *true* to display the field or *false* to hide it, or it |
|                        | angular expression| can be a angular expression that evaulates to *true* or *false*, for example,              |
|                        |                   | 5 > 2 would evaluate to *true* and 5 < 2 would evaluate to *false* because 5 is not less   |
|                        |                   | than 2.                                                                                    |
|                        |                   |                                                                                            |
|                        |                   | See :ref:`angular-expression-label`  for more help.                                        |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

.. include:: test-embed.rst

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

.. include:: webgc-props-events.rst

|


+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Add Directive**      | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
|  Extended Directives   | function name     | This allows you to add extended directives to customize the default Statictext and add     |
|                        |                   | functionality. When you click on *Add Directive*                                           |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+


|
|
