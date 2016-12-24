.. image:: ../../images/badges/badge_web.png
   :class: pull-right

Fab
===

.. image:: ../../images/icons/menu_fab.png
    :width: 50px
    :height: 50px


A Floating Action Button or **FAB** Menubar is a component included in Material Design guidelines that emphasizes the most
important action on the current screen usually on a mobile application. It is used to attract the users attention and perform
the primary action or the most intuitive action. The FAB Menubar opens a menu or an iconbar when the FAB is clicked on. It
can open to the right, left, up or down in respect to the button.

|

.. image:: ../../images/gcs/web/webgc-fab.png

When opened:

.. image:: ../../images/gcs/web/webgc-fab-menu.png

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

Try the Sample Fab

.. toctree::
   :maxdepth: 1

   ../../gsguide/samples/sample-fab

|

|

Reference
---------

The Fab control properties can be set for the following property categories:

* :ref:`webgc-fab-main-label`
* :ref:`webgc-fab-menu-label`
* :ref:`webgc-fab-render-label`
* :ref:`webgc-fab-styling-label`
* :ref:`webgc-fab-events-label`

|

Main Properties
^^^^^^^^^^^^^^

.. toctree::
   :maxdepth: 1

   webgc-prop-main-id
   webgc-prop-main-template
   webgc-prop-main-name
   webgc-prop-main-label
   webgc-prop-main-icon
   webgc-prop-main-display
   webgc-prop-main-disable

|

Styling Properties
^^^^^^^^^^^^^^^^^^

.. toctree::
   :maxdepth: 1

   webgc-prop-style-style
   webgc-prop-style-class
   webgc-prop-style-dynamic

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


.. _webgc-fab-menu-label:

FAB Menu
^^^^^^^^


+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Menu Items**         | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Static                 | Menu Editor       | Static means that the definition and contents of the menu/iconbar are static and once      |
|                        |                   | defined will remain the unchanged until they are manually changed again. The menu/iconbar  |
|                        |                   | can be defined by clicking on                                                              |
|                        |                   |        .. image:: ../../images/gcs/dfx-menu-edit-button.png                                |
|                        |                   | to bring the menu editor to assist in defining the menu/iconbar.                           |
|                        |                   |                                                                                            |
|                        |                   |                                                                                            |
|                        |                   |        .. image:: ../../images/gcs/dfx-help-menu-editor.png                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Dynamic                | NA                |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

.. _webgc-fab-render-label:

Rendering
^^^^^^^^^

This is the Rendering Section


.. _webgc-fab-styling-label:

FAB Styling Attributes
^^^^^^^^^^^^^^^^^^^^^^

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

.. _webgc-fab-events-label:

.. include:: webgc-events-focus.rst

Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.

|