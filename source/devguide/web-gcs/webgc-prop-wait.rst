Wait Properties
===============

This property sets the Icon that will show a wait status on the :term:`GC` while some action is running until its completion.
While the in wait mode the :term:`GC`can be disabled.

|

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Wait Properties**    | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Binding                | Scope Variable    | Beside the Static menu property is a **Edit** link to the Menu Editor. You define the Menu |
|                        | 'string'          | in the Menu Editor. Once you are satisfied you save the menu that has been defined.        |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Auto-Disabled          | *true* or *false* | Value is *true* to disable the :term:`GC` during the wait period or *false* to keep it     |
|                        | angular expression| active. The value can also be the result of an Boolean Angular Expression, see             |
|                        |                   | :ref:`angular-expression-label` for more details.                                          |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Icon                   | Name of Icon      | The name of the Font Awesome or SVG Icon to use in the wait. Enter the name in the property|
|                        |                   | field or click on **...** for a list to select from. See :ref:`dfx-icons-label`            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Icon Style             | CSS attributes    | Name of CSS class(es) separated by a space used for styling. For more detail see           |
|                        |                   | :ref:webgc-prop-style-label`                                                               |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Icon Class             | class name        | Name of CSS class(es) separated by a space used for styling. For more detail see           |
|                        |                   | :ref:webgc-prop-style-class-label`                                                         |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|