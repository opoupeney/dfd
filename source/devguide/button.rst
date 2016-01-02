Button
======

.. image:: ../images/icons/icon_web.png
   :class: pull-right

A button communicates an action to be performed when the user clicks on it. It consists of a label, an icon or both that
indicate the action to be performed when the button is clicked.

|

.. image:: ../images/gcs/dfx-button-designtime.png

|


Properties
^^^^^^^^^^

|

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Main Properties**    | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Name                   | btnButton#        | Name is a reference to the component's DOM element. It can be used to dynamically access   |
|                        |                   | and set component properties. DreamFace gives a default name of *btnButton#* where #       |
|                        |                   | corresponds to the order in which the control was created. The second button created       |
|                        |                   | will have a default Name of *btnButton2*. Name is not required and can be removed if not   |
|                        |                   | needed.                                                                                    |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| label                  | Any text or       | This is the text that will appear on the button indicating which  action that will         |
|                        | *expression*      | performed when the button is clicked. For example, the label might be *Cancel*, *OK*,      |
|                        |                   | *DEPLOY TO CLOUD*, or *ADD COMMENT*.                                                       |
|                        |                   |                                                                                            |
|                        |                   |        .. image:: ../images/gcs/dfx-button-label.png                                       |
|                        |                   |                                                                                            |
|                        |                   | **Labels can also be expressions** that are evaluated at runtime.                          |
|                        |                   |                                                                                            |
|                        |                   | See more about how to define :ref:`expressions-label` here.                                |
|                        |                   |                                                                                            |
|                        |                   | *Note* - Text needs to be in quotes otherwise it will be treated as a variable. If your    |
|                        |                   | label doesn't appear in Preview mode, make sure the text is in quotes. For words that      |
|                        |                   | contain an apostrophe, use double quotes. For example "It's a button" would evaluate to:   |
|                        |                   |                                                                                            |
|                        |                   | *It's a button* at runtime (in Preview Mode or when testing the application.               |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| icon                   | favicon           | Click on the **...** to the right of the field to select one of the favicons from the list.|
|                        |                   |                                                                                            |
|                        |                   |        .. image:: ../images/gcs/dfx-icons.png                                              |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| icon position          | *left* or *right* | *left* to display on the left and *right* to display on the right side of the button.      |
|                        |                   |                                                                                            |
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
| **Events**             | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| On Click               | function name     | Enter the name of the function that will be executed when the user clicks on the HTML      |
|                        |                   | control. The function should be defined in the controller in the script tab of the View    |
|                        |                   | Editor. Clicking on the ... opens a window to to select a function defined in the          |
|                        |                   | Controller.                                                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+


|
|

