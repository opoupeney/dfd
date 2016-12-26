.. image:: ../../images/badges/badge_web.png
    :class: pull-right

Chips
=====

.. image:: ../../images/icons/input_chips.png
    :width: 50px
    :height: 50px


Chips can be used for building lists of strings or entities, including free form text, predefined text, rules, or contacts.
Chips may also contain icons.

|

.. image:: ../../images/gcs/web/webgc-chips.png

|


See it in Action
----------------

Try the Sample Buttons

.. toctree::
   :maxdepth: 1

   ../../gsguide/samples/sample-chips

    |

|

Reference
---------



The Chips control properties can be set for the following property categories:

* :ref:`webgc-chips-main-label`
* :ref:`webgc-chips-render-label`
* :ref:`webgc-chips-styling-label`
* :ref:`webgc-chips-events-label`

|

.. _webgc-chips-main-label:


Main Properties
^^^^^^^^^^^^^^^

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


|

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Main Properties**    | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Name                   | chpChips#         | Name is a reference to the component's DOM element. It can be used to dynamically access   |
|                        |                   | and set component properties. DreamFace gives a default name of *chpChips#* where #        |
|                        |                   | corresponds to the order in which it was created. If it's the second chips control created |
|                        |                   | it will have a default Name of *chpChips2*. Name is not required and can be removed if not |
|                        |                   | needed.                                                                                    |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| label                  | Any text          | This is the text that will appear under the icon, for example the fa-home icon could have  |
|                        |                   | the label Home as DreamFace uses as the default for this component.                        |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| icon                   | favicon           | Click on the **...** to the right of the field to select one of the favicons from the list.|
|                        |                   |                                                                                            |
|                        |                   |        .. image:: ../../images/gcs/dfx-icons.png                                              |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Display                | *true* or *false* | *true* to display the field or *false* to hide it.                                         |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Disabled               | *true* or *false* | *true* to disable the field or *false* to make it active.                                  |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

.. _webgc-chips-render-label:

Rendering
^^^^^^^^^

This is the rendering section.


|

.. _webgc-chips-styling-label:


.. include:: webgc-styling-slider.rst

|


Events
^^^^^^

.. toctree::
   :maxdepth: 1

   webgc-events-chips.rst

Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.

|