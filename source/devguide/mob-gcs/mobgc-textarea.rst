.. image:: ../../images/badges/badge_mobile.png
   :class: pull-right

Textarea
========

The Textarea graphical control is a multi-line text input control. It can display an icon, can be set to required and can
have a maximum length set.

|

.. image:: ../../images/gcs/mob/mobgc-textarea.png

|

The Textarea Field control properties can be set for the following property categories:

* :ref:`mobgc-textarea-main-label`
* :ref:`mobgc-textarea-validation-label`
* :ref:`mobgc-textarea-styling-label`
* :ref:`mobgc-textarea-events-label`

|

.. _mobgc-textarea-main-label:

Main Properties
---------------

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

.. _mobgc-textarea-validation-label:

Validation Properties
---------------------

Validation Properties go here.

|

.. _mobgc-textarea-styling-label:

.. include:: mobgc-props-styling-slider.rst

|

.. _mobgc-textarea-events-label:

.. include:: mobgc-props-events-onchange.rst

Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.

|
