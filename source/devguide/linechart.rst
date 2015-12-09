Linechart
=========

.. image:: ../images/icons/icon_web.png
   :class: pull-right

|
Description
^^^^^^^^^^^

The pre-defined Charts graphical controls available in the Widget Editor are based on Angular Charts.

|

Properties
^^^^^^^^^^

**Main Properties**

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Main Properties        | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Name                   | chChart#          | Name is a reference to the component's DOM element. It can be used to dynamically access   |
|                        |                   | and set component properties. DreamFace gives a default name of *chChart#* where #         |
|                        |                   | corresponds to the order in which it was created. If it's the second accordion created it  |
|                        |                   | will have a default Name of *chChart2*. Name is not required and can be removed if not     |
|                        |                   | needed.                                                                                    |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Label                  | *text*            |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Label Visible          | *text*            | Text that will be displayed in the label of the field. Text can also be an expression.     |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Label Visible          | *yes*, *no*       | Specifies if the label is visible or not.                                                  |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Tooltips               | Any text          | Tip to help the user. It will be displayed when mouse passes over this control. Tooltip    |
|                        |                   | text can also be an expression.                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Type                   |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Labels for Data Points |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Inner Radius (Pie      |                   |                                                                                            |
| Charts                 |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Legend Visible         |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Legend Position        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

**Container CSS**

The Container CSS affects the style and presentation of the container that surrounds the component. For example the color of the container
will affect the text that is in the container like the label but not the text that is in the component.

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Container CSS          | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Classes                | CSS class         | Name of CSS class to use for the container of this component. The value can also be the    |
|                        | bootstrap class   | name of a bootstrap class.                                                                 |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Dynamic Classes        | CSS Class         | The Dynamic Class is a CSS or Bootstrap class that will be added to the container if an    |
|                        | Bootstap class    | Angular Express is verified. It is rendered as a ng-class attribute.                       |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Width                  | auto              | The width property sets the width of the container. Auto uses the default value for width. |
|                        | length in px / cm | Defines the height in px, cm. *example* - 100px or 10cm                                    |
|                        | percent           | Width expressed as a percentage of it's parent container.  *example* - 100%                |
|                        | initial           | The *initial* keyword sets a CSS property to its default value. *example* - initial        |
|                        | inherit           | The *inherit* keyword tells CSS property to inherit it's value from it's parent.           |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Height                 | auto              | The height property sets the height of the container. Auto sets height to its default value|
|                        | length in px / cm | Defines the height in px, cm. *example* - 100px or 10cm                                    |
|                        | percent           | Width expressed as a percentage of it's parent container.  *example* - 100%                |
|                        | initial           | The *initial* keyword sets a CSS property to its default value. *example* - initial        |
|                        | inherit           | The *inherit* keyword tells CSS property to inherit it's value from it's parent.           |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Color                  | #hexcode for color| CSS colors are defined using a hexadecimal (HEX) notation (see :term:`Hexadecimal Colors`) |
|                        | Predefined Cross- | or enter one of the Pre-defined cross browser colors.                                      |
|                        | Browser Colors    | `140 cross browser colors <http://www.w3schools.com/cssref/css_colornames.asp>`_           |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Background             | #hexcode for color| CSS colors are defined using a hexadecimal (HEX) notation (see :term:`Hexadecimal Colors`) |
|                        | Predefined Cross- | or enter one of the Pre-defined cross browser colors.                                      |
|                        | Browser Colors    | `140 cross browser colors <http://www.w3schools.com/cssref/css_colornames.asp>`_           |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Padding                | *length*, *%*     | Padding defines space between the content and the border of the container. Length defines  |
|                        |                   | the fixed paddingwhile percent defines the padding as a percentage of the container. When  |
|                        |                   | specifying length, pixels (px), centimeters (cm) and other units can be used *example* -   |
|                        |                   | 10px or 10cm. Default value is 0px. There are four values possible to set: top, left,      |
|                        |                   | bottom, and right, *example* - 10px 5px 10px 15px would set top and bottom to 10px and left|
|                        |                   | to 5px and right to 15px. Padding shorthand is accepted, for example 10px 5px would set    |
|                        |                   | padding on top and bottom to 10px and left and right to 5px. If only one value is specified|
|                        |                   | for length it is used for all four values, *example* - 20px would set all values to 20px.  |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Margin                 | *auto*, *length*, | Margin defines the space around the container. It is transparent and has no background     |
|                        | *%*, *inherit*    | Auto lets the browser calculate the margin, *example* - auto. When specifying the length   |
|                        |                   | pixels (px), centimeters (cm) and other units can be used *example* - 10px or 10cm.        |
|                        |                   | Default value is 0px. There are four values possible to set: top, left, bottom, and right  |
|                        |                   | and left margins to 0px. Margin shorthand is accepted, for example 10px 5px would set both |
|                        |                   | top and bottom margins to 10px and left and right to 5px.*%* specifies margin as           |
|                        |                   | percentage of its parent container, *example* - 100% to indicate to use the entire width of|
|                        |                   | the parent. *inherit* indicates that the value will be inherited from its parent,          |
|                        |                   | *example* - inherit.                                                                       |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Text Algnment          | *left*, *center*, | Specifies alignment of container text on left, center or right.                            |
|                        | *right*           |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Custom CSS             | CSS Class         | Custom CSS provides a way to set CSS properties for which DreamFace does not expressly     |
|                        | Bootstrap class   | provide a way to set. *example - border-style: solid; border-width: 5px puts a solid border|
|                        |                   | around the container.                                                                      |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

**Component CSS**

The Component CSS is the CSS that affects the style of the component itself.


+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Component CSS          | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Classes                | CSS class         | Name of CSS class to use for the container of this component. The value can also be the    |
|                        | bootstrap class   | name of a bootstrap class.                                                                 |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Dynamic Classes        | CSS Class         | The Dynamic Class is a CSS or Bootstrap class that will be added to the container if an    |
|                        | Bootstap class    | Angular Express is verified. It is rendered as a ng-class attribute.                       |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Width                  | auto              | The width property sets the width of the component. Auto uses the default value for width. |
|                        | length in px / cm | Defines the height in px, cm. *example* - 100px or 10cm                                    |
|                        | percent           | Width expressed as a percentage of it's parent container.  *example* - 100%                |
|                        | initial           | The *initial* keyword sets a CSS property to its default value. *example* - initial        |
|                        | inherit           | The *inherit* keyword tells CSS property to inherit it's value from it's parent.           |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Height                 | auto              | The height property sets the height of the component. Auto sets height to its default value|
|                        | length in px / cm | Defines the height in px, cm. *example* - 100px or 10cm                                    |
|                        | percent           | Width expressed as a percentage of it's parent container.  *example* - 100%                |
|                        | initial           | The *initial* keyword sets a CSS property to its default value. *example* - initial        |
|                        | inherit           | The *inherit* keyword tells CSS property to inherit it's value from it's parent.           |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Color                  | #hexcode for color| CSS colors are defined using a hexadecimal (HEX) notation (see :term:`Hexadecimal Colors`) |
|                        | Predefined Cross- | or enter one of the Pre-defined cross browser colors.                                      |
|                        | Browser Colors    | `140 cross browser colors <http://www.w3schools.com/cssref/css_colornames.asp>`_           |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Background             | #hexcode for color| CSS colors are defined using a hexadecimal (HEX) notation (see :term:`Hexadecimal Colors`) |
|                        | Predefined Cross- | or enter one of the Pre-defined cross browser colors.                                      |
|                        | Browser Colors    | `140 cross browser colors <http://www.w3schools.com/cssref/css_colornames.asp>`_           |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Padding                | *length*, *%*     | Padding defines space between the content and the border of the component. Length defines  |
|                        |                   | the fixed paddingwhile percent defines the padding as a percentage of the container. When  |
|                        |                   | specifying length, pixels (px), centimeters (cm) and other units can be used *example* -   |
|                        |                   | 10px or 10cm. Default value is 0px. There are four values possible to set: top, left,      |
|                        |                   | bottom, and right, *example* - 10px 5px 10px 15px would set top and bottom to 10px and left|
|                        |                   | to 5px and right to 15px. Padding shorthand is accepted, for example 10px 5px would set    |
|                        |                   | padding on top and bottom to 10px and left and right to 5px. If only one value is specified|
|                        |                   | for length it is used for all four values, *example* - 20px would set all values to 20px.  |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Margin                 | *auto*, *length*, | Margin defines the space around the component. It is transparent and has no background     |
|                        | *%*, *inherit*    | Auto lets the browser calculate the margin, *example* - auto. When specifying the length   |
|                        |                   | pixels (px), centimeters (cm) and other units can be used *example* - 10px or 10cm.        |
|                        |                   | Default value is 0px. There are four values possible to set: top, left, bottom, and right  |
|                        |                   | and left margins to 0px. Margin shorthand is accepted, for example 10px 5px would set both |
|                        |                   | top and bottom margins to 10px and left and right to 5px.*%* specifies margin as           |
|                        |                   | percentage of its parent container, *example* - 100% to indicate to use the entire width of|
|                        |                   | the parent. *inherit* indicates that the value will be inherited from its parent,          |
|                        |                   | *example* - inherit.                                                                       |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Text Algnment          | *left*, *center*, | Specifies alignment of component text on left, center or right.                            |
|                        | *right*           |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Custom CSS             | CSS Class         | Custom CSS provides a way to set CSS properties for which DreamFace does not expressly     |
|                        | Bootstrap class   | provide a way to set. *example - border-style: solid; border-width: 5px puts a solid border|
|                        |                   | around the container.                                                                      |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|
**Events**