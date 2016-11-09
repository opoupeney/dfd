Styling Attributes
^^^^^^^^^^^^^^^^^^

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Styling Attributes** |                   |                                                                                 |
+========================+===================+============================================================================================+
| **Container Stylings** | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Style                  | CSS syles         | CSS style attribure(s) to use for this component, separated by semi-colons, for example:   |
|                        |                   | *color:red; background-color:lightgray*. By clicking on the **...** on the right hand side |
|                        |                   | of the field, a window opens up proposing to change attributes for **font**, **color**,    |
|                        |                   | **padding** and **margin** presented in a tree. When clicking on the arrow to the left of  |
|                        |                   | the attribute type, the user is guide by placeholder to enter the correct settings         |
|                        |                   |                                                                                            |
|                        |                   |        .. image:: ../../images/gcs/dfx-styles-editor.png                                   |
|                        |                   |           :width: 450px                                                                    |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Class                  | CSS class         | Name of CSS class to use for the component.                                                |
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
|                        |                   |            .RedMessage {                                                                   |
|                        |                   |                   color: red                                                               |
|                        |                   |                }                                                                           |
|                        |                   |                                                                                            |
|                        |                   |   Dynamic class could be an angular expression like                                        |
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
+========================+===================+============================================================================================+
| **Icon Stylings**      | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Size                   | number in pixels  | This number represents the width of the slider in pixels. The default value is 500.        |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Style                  | CSS syles         | CSS style attribure(s) to use for this component, separated by semi-colons, for example:   |
|                        |                   | *color:red; background-color:lightgray*. By clicking on the **...** on the right hand side |
|                        |                   | of the field, a window opens up proposing to change attributes for **font**, **color**,    |
|                        |                   | **padding** and **margin** presented in a tree. When clicking on the arrow to the left of  |
|                        |                   | the attribute type, the user is guide by placeholder to enter the correct settings         |
|                        |                   |                                                                                            |
|                        |                   |        .. image:: ../../images/gcs/dfx-styles-editor.png                                   |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Classes                | CSS class         | Name of CSS class to use for the component.                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Item Stylings**      | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Style                  | CSS syles         | CSS style attribure(s) to use for this component, separated by semi-colons, for example:   |
|                        |                   | *color:red; background-color:lightgray*. By clicking on the **...** on the right hand side |
|                        |                   | of the field, a window opens up proposing to change attributes for **font**, **color**,    |
|                        |                   | **padding** and **margin** presented in a tree. When clicking on the arrow to the left of  |
|                        |                   | the attribute type, the user is guide by placeholder to enter the correct settings         |
|                        |                   |                                                                                            |
|                        |                   |        .. image:: ../../images/gcs/dfx-styles-editor.png                                   |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Classes                | CSS class         | Name of CSS class to use for the component.                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Icon Size              | number in pixels  | This number represents the width of the slider in pixels. The default value is 500.        |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Icon Style             | CSS syles         | CSS style attribure(s) to use for this component, separated by semi-colons, for example:   |
|                        |                   | *color:red; background-color:lightgray*. By clicking on the **...** on the right hand side |
|                        |                   | of the field, a window opens up proposing to change attributes for **font**, **color**,    |
|                        |                   | **padding** and **margin** presented in a tree. When clicking on the arrow to the left of  |
|                        |                   | the attribute type, the user is guide by placeholder to enter the correct settings         |
|                        |                   |                                                                                            |
|                        |                   |        .. image:: ../../images/gcs/dfx-styles-editor.png                                   |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Icon Class             | CSS class         | Name of CSS class to use for the component.                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+


|