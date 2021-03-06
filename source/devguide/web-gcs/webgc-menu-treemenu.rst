.. image:: ../../images/badges/badge_web.png
   :class: pull-right

Treemenu
========

.. image:: ../../images/icons/menu_treemenu.png
    :width: 50px
    :height: 50px


The TreeMenu graphical control presents a menu as a list of links in a hierarchical tree format of menus and submenus. The
subitems are indentated showing that they are sub-categories of the parent node. These submenus can be expanded or collapsed
to show sub menus by the user with icons (usually '+' and '-' or other icons) that indicate if a branch is expanded or collapsed.

A Treemenu can have a static or dynamic representation.

|

.. image:: ../../images/gcs/web/webgc-treemenu.png

|

Detailed Treemenu Reference
---------------------------

The Treemenu control properties can be set for the following property categories:

Main Properties
^^^^^^^^^^^^^^

.. toctree::
   :maxdepth: 1

   webgc-prop-main-id
   webgc-prop-main-template
   webgc-prop-main-name
   webgc-prop-main-display
   webgc-prop-main-menuitems

|

Styling Attributes
^^^^^^^^^^^^^^^^^^

Container Stying
''''''''''''''''

.. toctree::
   :maxdepth: 1

   webgc-prop-style-style
   webgc-prop-style-class
   webgc-prop-style-dynamic

|

Menu Stying
'''''''''''

.. toctree::
   :maxdepth: 1

   webgc-prop-style-style
   webgc-prop-style-class
   webgc-prop-style-iconsize
   webgc-prop-style-iconstyle
   webgc-prop-style-iconclass

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


Events
^^^^^^

.. toctree::
   :maxdepth: 1

   webgc-events.rst

|


**How to create a treemenu**

+----------------------------------------------------------------------------------------+-------------------------------------------------------+
| **Step Descriptions**                                                                  | Screen                                                |
+========================================================================================+=======================================================+
| Drag and drop Treemenu GC to the working area, click on GC and then                    | .. figure:: ../../images/gcs/dfx-help-css-styles.png  |
| open Menu editor in popup by cliking Edit button in Property Panel.                    |     :width: 150px                                     |
| You’ll see default item: ‘Home’                                                        |     :height: 75px                                     |
+----------------------------------------------------------------------------------------+-------------------------------------------------------+

See it in Action
----------------

Try the Sample Treemenu controls

.. toctree::
   :maxdepth: 1

   ../../gsguide/samples/sample-treemenu

|

Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.
