.. image:: ../../images/icons/badge_web.png
   :class: pull-right

Textarea
========

The Textarea graphical control is a multi-line text input control. A *Textarea* can contain an unlimited number of characters,
and text renders in a fixed-width font. allows a developer to add any custom HTML. The contents of the HTML field is pure HTML. By
default the control contains a Lorem Ipsum text. This contect can be edited to include any HTML content. For example,
if you find that one of the pre-defined graphical controls does not have the functionality that you need, you can add
your own in the HTML control.

The <textarea> tag defines a multi-line text input control.

A text area can hold an unlimited number of characters, and the text renders in a fixed-width font (usually Courier).

The size of a text area can be specified by the cols and rows attributes, or even better; through CSS' height and width properties.

|

.. image:: ../../images/gcs/web/webgc-textarea.png

|

The Textarea Field control properties can be set for the following property categories:

* :ref:`webgc-textarea-main-label`
* :ref:`webgc-textarea-validation-label`
* :ref:`webgc-textarea-styling-label`
* :ref:`webgc-textarea-events-label`

|

.. _webgc-textarea-main-label:

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

.. _webgc-textarea-validation-label:

Validation Properties
---------------------

Validation Properties go here.

|

.. _webgc-textarea-styling-label:

.. include:: webgc-props-styling-slider.rst

|

.. _webgc-textarea-events-label:

.. include:: webgc-props-events-onchange.rst


|
|

