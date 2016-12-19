.. image:: ../../images/badges/badge_web.png
   :class: pull-right

Statictext
==========

.. image:: ../../images/icons/basic_statictext.png
    :width: 50px
    :height: 50px

A **statictext** is a graphical control which displays text that cannot be directly modified by the user. It is not
interactive and does not require any user input. Statictext controls often serve as labels for other controls or to
identify different sections of the View. They can also be used to add context to the user interface.

|

.. image:: ../../images/gcs/web/webgc-statictext.png

|

Features
--------
* Complete Styling with CSS, CSS Classes or Dynamic Classes
* Dynamic Hide or Show Capabilies
* Easy Tooltip setting and tooltip positionning
* Full set of Events (ie. On Click or Mouse Over, ...)

|

See it in Action
----------------

Try some Sample Statictext controls

.. toctree::
   :maxdepth: 1

   ../../gsguide/samples/sample-statictext

|

Reference
---------

The Statictext control can define the following categories of properties:

* :ref:`webgc-text-main-label`
* :ref:`webgc-text-styling-label`
* :ref:`webgc-text-tooltip-label`
* :ref:`webgc-text-events-label`

|

.. _webgc-text-main-label:

.. include:: webgc-properties-main.rst

|

.. _webgc-text-styling-label:

.. include:: webgc-styling.rst

|

.. _webgc-text-tooltip-label:

Tooltip Properties
^^^^^^^^^^^^^^^^^^

Tooltip properties allow us to set the text and style of the tooltip that will appear when we hover the mouse over the
:term:`GC`.

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Tooltip Properties** | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Text                   | 'string' or       | This is the text of the tooltip which contains instructions to help the user know what to  |
|                        | scope variable or | do. It will be displayed when mouse passes over the :term:`GC`. The Text can also be an    |
|                        | angular expression| expression,`for example 'this is the tool' + 'TIP' would display *this is the toolTIP*.    |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Direction              | Left, Top,        | The value of this field indicates where the tooltip text will appear. A radio button is    |
|                        | Bottom, Right     | provided with the values Left, Top, Bottom or Right corresponding to the position where the|
|                        |                   | tooltip will be displayed relative to the :term:`GC`.                                      |
|                        |                   |                                                                                            |
|                        |                   |   .. image:: ../../images/gcs/web/wgc-statictext-tooltip-direction.png                     |
|                        |                   |      :width: 400px                                                                         |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Style                  | CSS syles         | CSS style attribure(s) to use for this component, separated by semi-colons, for example:   |
|                        |                   | *color:red; background-color:lightgray*. By clicking on the **...** on the right hand side |
|                        |                   | of the field, a window opens up proposing to change attributes for **font**, **color**,    |
|                        |                   | **padding** and **margin** presented in a tree. When clicking on the arrow to the left of  |
|                        |                   | the attribute type, the user is guide by placeholder to enter the correct settings         |
|                        |                   |                                                                                            |
|                        |                   |   .. image:: ../../images/gcs/dfx-styles-editor.png                                        |
|                        |                   |      :width: 300px                                                                         |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Class                  | CSS class         | Name of CSS class(es) separated by a space, to use to style the :term:`GC`.                |
|                        |                   | For more on styling :term:`GC`s see :ref:`gcs-styling-label`                               |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

See :ref:`gcs-styling-label`


.. _webgc-text-events-label:

.. include:: webgc-events.rst

|

Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.

|
