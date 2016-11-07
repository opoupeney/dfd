.. image:: ../../images/badges/badge_web.png
   :class: pull-right

Textarea
========

.. image:: ../../images/icons/input_textarea.png
    :width: 50px
    :height: 50px


The Textarea graphical control is a multi-line text input control. It can display an icon, can be set to required and can
have a maximum length set.

|

.. image:: ../../images/gcs/web/webgc-textarea.png

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

Try the Sample Buttons

.. toctree::
   :maxdepth: 1

   ../../gsguide/samples/sample-textarea

    |

|

Reference
---------

The Textarea Field control properties can be set for the following property categories:

* :ref:`webgc-textarea-main-label`
* :ref:`webgc-textarea-validation-label`
* :ref:`webgc-textarea-render-label`
* :ref:`webgc-textarea-styling-label`
* :ref:`webgc-textarea-events-label`

|

.. _webgc-textarea-main-label:

Main Properties
^^^^^^^^^^^^^^

|

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Main Properties**    | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Name                   | htHtml#           | Name is a reference to the component's DOM element. It can be used to dynamically access   |
|                        |                   | and set component properties. DreamFace gives a default name of *htHtml* where #           |
|                        |                   | corresponds to the order in which the control was created. If it's the second control      |
|                        |                   | created it will have a default Name of *htHtml12*. Name is not required and can be removed |
|                        |                   | if not needed.                                                                             |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Binding                | Any text          | The HTML control can be bound to data coming from a service, for example a service that    |
|                        |                   | goes to a content management system. Text that will be displayed in the field.             |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Content                | Any HTML text     | The content can be edited to enter any HTML text manually in a contextual script editor.   |
|                        |                   | The new content will be displayed as soon as it is saved.                                  |
|                        |                   |                                                                                            |
|                        |                   |        .. image:: ../../images/gcs/dfx-html-editor.png                                     |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Display                | *true* or *false* | *true* to display the field or *false* to hide it.                                         |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Disabled               | *true* or *false* | *true* to disable the field or *false* to make it active.                                  |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

|

.. _webgc-textarea-validation-label:

Validation Properties
^^^^^^^^^^^^^^^^^^^^^

Validation Properties go here.

|

.. _webgc-textarea-render-label:

Rendering
^^^^^^^^^

This is the rendering section.


|

.. _webgc-textarea-styling-label:

.. include:: webgc-styling-slider.rst

|

.. _webgc-textarea-events-label:

.. include:: webgc-events-onchange.rst

Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.

|

