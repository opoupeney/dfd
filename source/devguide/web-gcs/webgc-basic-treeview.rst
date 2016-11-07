.. image:: ../../images/badges/badge_web.png
   :class: pull-right

Treeview
========

.. image:: ../../images/icons/basic_treeview.png
    :width: 50px
    :height: 50px


A treeview is a graphical control that presents information in a hierarchical view. Each item (often referred to
as a branch or a node) can have a number of subitems or children. The subitems or children are often visualized by indentation
in a list showing that they are sub-categories of the parent node. Items can be expanded to show subitems and
collapsed to hide subitems.

An example of a Treeview that most people are familiar with is file directories with folders, sub-folers and individual
files allowing users to organize and easily find files.

|

.. image:: ../../images/gcs/web/webgc-treeview.png

|

Features
--------
* Feature 1
* Feature 2
* Feature 3
* Feature 4

|

See it in Action
----------------

Try the Sample Treeviews

.. toctree::
   :maxdepth: 1

   ../../gsguide/samples/sample-treeviews

|

Reference
---------


The Treeview control properties can be set for the following property categories:

* :ref:`webgc-treeview-main-label`
* :ref:`webgc-treeview-menu-label`
* :ref:`webgc-treeview-render-label`
* :ref:`webgc-treeview-styling-label`
* :ref:`webgc-treeview-events-label`

|

.. _webgc-treeview-main-label:

Main Properties
^^^^^^^^^^^^^^

|

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Main Properties**    | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Name                   | fbFAB#            | Name is a reference to the component's DOM element. It can be used to dynamically access   |
|                        |                   | and set component properties. DreamFace gives a default name of *fbFAB#* where #           |
|                        |                   | corresponds to the order in which the control was created. The second FAB control created  |
|                        |                   | will have a default Name of *fbFAB2*. Name is not required and can be removed if not       |
|                        |                   | needed.                                                                                    |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Direction              | *right* or *left* | The direction of the associated menu or iconbar when the FAB is clicked. Choose one of the |
|                        | *up* or *down*    | proposed values *Right*, *Left*, *Up* or *Down*.                                           |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Animation Mode         | *Fling* or *Scale*| The value can either *Fling* or *Scale*. Fling means ... Scale means ...                   |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Menu Icon              | `Name of the      | The value can either be a literal *true* to display the field or *false* to hide it. It can|
|                        | favicon`          | also be a angular expression that evaulates to *true* or *false*, for example,             |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Display                | *true* or *false* | The value can either be a literal *true* to display the field or *false* to hide it, or it |
|                        | angular expression| be a angular expression that evaulates to *true* or *false*, for example,                  |
|                        |                   |                                                                                            |
|                        |                   | 5 > 2 would evaluate to *true* and 5 < 2 would evaluate to false.                          |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Disabled               | *true* or *false* | The value can either be a literal *true* to display the field or *false* to hide it, or it |
|                        | angular expression| be a angular expression that evaulates to *true* or *false*, for example,                  |
|                        |                   |                                                                                            |
|                        |                   | 5 > 2 would evaluate to *true* and 5 < 2 would evaluate to false.                          |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

.. _webgc-treeview-menu-label:

Menu Items
^^^^^^^^^^

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Menu Items**         | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Static                 | Menu Editor       | Static means that the definition and contents of the menu/iconbar are static and once      |
|                        |                   | defined will remain the unchanged until they are manually changed again. The menu  |
|                        |                   | can be defined by clicking on                                                              |
|                        |                   |        .. image:: ../images/gcs/dfx-menu-edit-button.png                                   |
|                        |                   | to bring the menu editor to assist in defining the menu/iconbar.                           |
|                        |                   |                                                                                            |
|                        |                   |                                                                                            |
|                        |                   |        .. image:: ../../images/gcs/dfx-help-menu-editor.png                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Dynamic                | NA                |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

.. _webgc-treeview-render-label:

Rendering
^^^^^^^^

This is the rendering section.

|

.. _webgc-treeview-styling-label:

Styling Attributes
^^^^^^^^^^^^^^^^^

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Styling Attributes** | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Style                  | CSS syles         | CSS style attribure(s) to use for this component, separated by semi-colons, for example:   |
|                        |                   | *color:red; background-color:lightgray*. By clicking on the **...** on the right hand side |
|                        |                   | of the field, a window opens up proposing to change attributes for **font**, **color**,    |
|                        |                   | **padding** and **margin** presented in a tree. When clicking on the arrow to the left of  |
|                        |                   | the attribute type, the user is guide by placeholder to enter the correct settings         |
|                        |                   |                                                                                            |
|                        |                   |        .. image:: ../../images/gcs/dfx-help-css-styles.png                                 |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Menu Style             | CSS class         | Name of CSS class to use for the component.                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Menu Icon Style        | CSS class         | Name of CSS class to use for the component.                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Item Style             | CSS class         | Name of CSS class to use for the component.                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Item Icon Style        | CSS class         | Name of CSS class to use for the component.                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Item Class             | CSS class         | Name of CSS class to use for the component.                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Dynamic Class          | CSS Class         | The Dynamic Class is a CSS class that will be added to the graphical control if an Angular |
|                        |                   | Expression is verified. It is rendered as a ng-class attribute.                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

.. _webgc-treeview-events-label:

.. include:: webgc-events.rst

|


How to create a treeview
^^^^^^^^^^^^^^^^^^^^^^^

The TreeView Graphical Control can be bound to a JSON.  The JSON can have a repetitive child property:

Ex: a directory structure
[{
    "name": "’default’",
    "children": [{
        "name": "’products’",
        "children": [
            { "name": "’Printers’",
  "children": [
    { “name”: “‘Canon’” },
    { “name”: “‘HP’” },
    { “name”: “‘Samsung’” }
] },
            { "name": "’Scanners’",
 "children": [] }
        ]
    }]
}]

TreeView can be static/dynamic. Dynamic representation has higher priority then static.
Static representation
Static representation can be build with popup dialog window like GC Iconbar/Fab/Treemenu. In popup window we can set labels for each item. Labels are expressions.
Dynamic representation
It can work with json object of different structure. Need to put three parameters into TreeView items section fields of Property Panel:
Dynamic - it is name of scope array;
Repeatable Property - name of repeatable scope array property;
Label - name of property that will be TreeView item label.

Example:

$scope.treeview = [{
    "asd": "'default ' + symbol",
    "quantity": "'045'",
    "url": "http://google.com.ua",
    "qwe": [
      {
        "asd": "'products'",
        "qwe": [
          {
            "asd": "'Printers'",
            "qwe": []
          }
        ]
      }
    ]
  }]

To bind it to GC TreeView we need set in Property Panel:
Dynamic - treeview;
Repeatable Property - qwe;
Label - asd.

GC TreeView has special 3 styling properties:
Icon if Opened ( expression, default: ‘fa-minus’ ) - it is icon for item which is “opened/expanded” (when children are displayed);
Icon if Closed ( expression, default: ‘fa-plus’ ) - it is icon for item which is “closed/collapsed” (when children are hided);
Icon color ( css color value ) - it is icons color.
Icons can be changed in popup window or as a scope variable.
For example, for “opened” in popup window select ‘fa-folder-open’ and for “closed” - ‘fa-folder’, Icon color - green.

Those icons are clickable and can only expande/collapse item children.

To Each GC TreeView item we can connect events from Property Panel.

For example we have simple function in scope:

$scope.clickedItem = function(item) {
	console.log(item);
};
And we put into ‘On Double click’ field: selectNode($dfx_item).
As a result in console we will see our doubleClicked item ( an object with all his properties  ).



+----------------------------------------------------------------------------------------+-------------------------------------------------------+
| **Step Descriptions**                                                                  | Screen                                                |
+========================================================================================+=======================================================+
| Drag and drop Treemenu GC to the working area, click on GC and then                    | .. figure:: ../../images/gcs/dfx-help-css-styles.png  |
| open Menu editor in popup by cliking Edit button in Property Panel.                    |     :width: 150px                                     |
| You’ll see default item: ‘Home’                                                        |     :height: 75px                                     |
+----------------------------------------------------------------------------------------+-------------------------------------------------------+

Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.

|
