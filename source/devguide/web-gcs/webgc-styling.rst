Styling Attributes
^^^^^^^^^^^^^^^^^^

By setting Styling Properties it is possible to add CSS styles, classes and dynamic classes to style the graphical control.

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Styling Attributes** | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Style                  | CSS syles         | CSS style attributes can be added directly into this field, each separated by a semi-colon |
|                        | attribute:value   | for example *color:red; background-color:lightgray; padding-top:5px;* or by clicking on    |
|                        | separated by ;    | the **...** on the right side of the field, a help view opens up proposing to guide the    |
|                        |                   | the developer in CSS attribute setting. You can navigate the different sections  for       |
|                        |                   | **font**, **padding**, **margin**, etc. and set the desired attributes, guided by          |
|                        |                   | placeholder values to help enter the correct settings. When you click on *Save* the values |
|                        |                   | populate the Styles property field.                                                        |
|                        |                   |                                                                                            |
|                        |                   |        .. image:: ../../images/gcs/dfx-styles-editor.png                                   |
|                        |                   |           :width: 400px                                                                    |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Class                  | CSS class         | Name of CSS class to use for the component. The class can be defined in the DreamFace      |
|                        | separated by space| Styles or imported in a CSS file in the Resource Editor in the Applicaiton configuration   |
|                        |                   | parameters.                                                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Dynamic Classes        | CSS Class         | The Dynamic Class is a CSS class that will be added to the graphical control if an Angular |
|                        |                   | Expression is verified.                                                                    |
|                        |                   |                                                                                            |
|                        |                   |                                                                                            |
|                        |                   |                                                                                            |
|                        |                   | Consider the following CSS class:                                                          |
|                        |                   | ::                                                                                         |
|                        |                   |                                                                                            |
|                        |                   |  .RedMessage {                                                                             |
|                        |                   |     color:red;                                                                             |
|                        |                   |   }                                                                                        |
|                        |                   |                                                                                            |
|                        |                   |   Dynamic class could be an angular expression like                                        |
|                        |                   |                                                                                            |
|                        |                   |  RedMessage: my_variable<0                                                                 |
|                        |                   |                                                                                            |
|                        |                   | Another example might be:                                                                  |
|                        |                   | ::                                                                                         |
|                        |                   |                                                                                            |
|                        |                   |  .RedValue {                                                                               |
|                        |                   |      color: red;                                                                           |
|                        |                   |  }                                                                                         |
|                        |                   |  .GreenValue {                                                                             |
|                        |                   |      color: green;                                                                         |
|                        |                   |  }                                                                                         |
|                        |                   |                                                                                            |
|                        |                   |  Dynamic class could be an angular expression like                                         |
|                        |                   |                                                                                            |
|                        |                   |   RedValue: my_variable<0; GreenValue: my_variable>=0                                      |
|                        |                   |                                                                                            |
|                        |                   |   depending on the value of my_variable, the component will have the RedValue class        |
|                        |                   |   or GreenValue class. The goal is to change an attribute dynamically using angular        |
|                        |                   |   and not the DOM.                                                                         |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|