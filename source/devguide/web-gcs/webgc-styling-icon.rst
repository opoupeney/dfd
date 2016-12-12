Container Styling
^^^^^^^^^^^^^^^^^

 .. image:: ../../images/gcs/dfx-vieweditor-styles-container.png

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Styling Attributes** | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Size width to Label    | check /not checked| If Size width to Label is checked the width of the control will be adjusted to be the      |
|                        |                   |           :width: 400px                                                                    |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Style                  | CSS syles         | CSS styles attributes can be added directly into this field, each separated by a semi-colon|
|                        |                   | for example *color:red; background-color:lightgray*. By clicking on the **...** on the     |
|                        |                   | hand side of the field, a help view opens up proposing to change attributes. You can       |
|                        |                   | navigate the different sections  for **font**, **padding**, **margin**, etc. and set the   |
|                        |                   | the attributes that you need, guided by placeholder value to help enter the correct        |
|                        |                   | settings. When you save the values populate the Styles property field.                     |
|                        |                   |                                                                                            |
|                        |                   |        .. image:: ../../images/gcs/dfx-styles-editor.png                                   |
|                        |                   |           :width: 400px                                                                    |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Class                  | CSS class         | Name of CSS class to use for the component. The class can be defined in the DreamFace      |
|                        |                   | Styles or imported in a CSS file in the Resource Editor in the Applicaiton configuration   |
|                        |                   | parameters.                                                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Dynamic Classes        | CSS Class         | The Dynamic Class is a CSS class that will be added to the graphical control if an Angular |
|                        |                   | Expression is verified.                                                                    |
|                        |                   |                                                                                            |
|                        |                   | Consider the following CSS class:                                                          |
|                        |                   | ::                                                                                         |
|                        |                   |                                                                                            |
|                        |                   |     .RedMessage {                                                                          |
|                        |                   |         color: red                                                                         |
|                        |                   |        }                                                                                   |
|                        |                   |                                                                                            |
|                        |                   | Consider the following CSS class:                                                          |
|                        |                   | ::                                                                                         |
|                        |                   |                                                                                            |
|                        |                   |                                                                                            |
|                        |                   | Dynamic class could be an angular expression like                                          |
|                        |                   |                                                                                            |
|                        |                   |             *RedMessage: my_variable<0*                                                    |
|                        |                   |                                                                                            |
|                        |                   |                  --- or another example might be ---                                       |
|                        |                   |                                                                                            |
|                        |                   |            .RedValue {                                                                     |
|                        |                   |                    color: red;                                                             |
|                        |                   |                }                                                                           |
|                        |                   |            .GreenValue {                                                                   |
|                        |                   |                    color: green;                                                           |
|                        |                   |                }                                                                           |
|                        |                   |                                                                                            |
|                        |                   |   Dynamic class could be an angular expression like                                        |
|                        |                   |                                                                                            |
|                        |                   |             RedValue: my_variable<0; GreenValue: my_variable>=0                            |
|                        |                   |                                                                                            |
|                        |                   |   depending on the value of my_variable, the component will have the RedValue class        |
|                        |                   |   or GreenValue class. The goal is to change an attribute dynamically using angular        |
|                        |                   |   and not the DOM.                                                                         |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|