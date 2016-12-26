.. image:: ../../images/badges/badge_web.png
   :class: pull-right

Input Field
===========

.. image:: ../../images/icons/input_input.png
    :width: 50px
    :height: 50px


The Input graphical control is a single-line input field where users can enter data.

|

.. image:: ../../images/gcs/web/webgc-input.png

|

See it in Action
----------------

Try the Sample Iconss

.. toctree::
   :maxdepth: 1

   ../../gsguide/samples/sample-input

|

Reference
---------

The Input Field control properties can be set for the following property categories:


* :ref:`webgc-input-validation-label`
* :ref:`webgc-input-render-label`
* :ref:`webgc-input-styling-label`
* :ref:`webgc-input-events-label`

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
   webgc-prop-main-disabled

|

Styling Attributes
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
| Name                   | inpInput#         | Name is a reference to the component's DOM element. It can be used to dynamically access   |
|                        |                   | and set component properties. DreamFace gives a default name of *inpInput#* where #        |
|                        |                   | corresponds to the order in which the control was created. If it's the second input field  |
|                        |                   | created it will have a default Name of *inpInput2*. Name is not required and can be removed|
|                        |                   | if not needed.                                                                             |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| label                  | Any text          | This is the text that will appear under the icon, for example the fa-home icon could have  |
|                        |                   | the label Home as DreamFace uses as the default for this component.                        |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| icon                   | favicon           | Click on the **...** to the right of the field to select one of the favicons from the list.|
|                        |                   |                                                                                            |
|                        |                   |        .. image:: ../../images/gcs/dfx-icons.png                                           |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Display                | *true* or *false* | The value can either be a literal *true* to display the field or *false* to hide it, or it |
|                        | angular expression| be a angular expression that evaulates to *true* or *false*, for example,                  |
|                        |                   |                                                                                            |
|                        |                   | 5 > 2 would evaluate to *true* and 5 < 2 would evaluate to false                           |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Disabled               | *true* or *false* | *true* to disable the field or *false* to make it active or it be a angular expression that|
|                        | angular expression| evaulates to *true* or *false*, for example,                                               |
|                        |                   |                                                                                            |
|                        |                   | 5 > 2 would evaluate to *true* and 5 < 2 would evaluate to false                           |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

.. include:: webgc-properties-main-generic.rst


.. _webgc-input-validation-label:

Validation Properties
^^^^^^^^^^^^^^^^^^^^^

Validation Properties

|

.. _webgc-input-render-label:

Rendering
^^^^^^^^^

This is the rendering section.

|

.. _webgc-input-styling-label:

.. include:: webgc-styling-slider.rst

|

.. _webgc-input-events-label:

.. include:: webgc-events-onchange.rst

Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.

|