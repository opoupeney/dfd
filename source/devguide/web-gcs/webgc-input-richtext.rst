.. image:: ../../images/badges/badge_web.png
   :class: pull-right

Richtext
========

.. image:: ../../images/icons/input_richtext.png
    :width: 50px
    :height: 50px


A richtext control provides a number of properties you can be used to apply formatting to any portion of text within the
control in a view at runtime of your application.

To change the formatting of text, selecct the part of the text to format and assign the desired formatting.
Using formatting, you can make text bold or italic, change the color, font and many other styles.

|

.. image:: ../../images/gcs/web/webgc-richtext.png

|

Richtext Reference
------------------

The Richtext control properties can be set for the following property categories:

Main Properties
^^^^^^^^^^^^^^

.. toctree::
   :maxdepth: 1

   webgc-prop-main-id
   webgc-prop-main-template
   webgc-prop-main-name
   webgc-prop-main-whiteframe
   webgc-prop-main-binding
   webgc-prop-main-display
   webgc-prop-main-disabled

|

Toolbar Properties
^^^^^^^^^^^^^^^^^^
.. toctree::
   :maxdepth: 1

   webgc-prop-toolbar

|

Styling Attributes
^^^^^^^^^^^^^^^^^^

.. toctree::
   :maxdepth: 1

   webgc-prop-style-flexwidth
   webgc-prop-style-style
   webgc-prop-style-class
   webgc-prop-style-dynamic

|


+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Main Properties**    | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
|Title                   | Any text          | Title text or expression defines title of the panel.                                       |
|                        | Angular Expression|                                                                                            |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Title Visible          | Boolean value     | Title visible can either be set directly using *true* or *false* values or can be the      |
|                        | Angular Expression| result of an angular expression that returns a boolean value of the true or false, $true*  |
|                        |                   | meaning the title will be visible, *false* meaning title will not be displayed.            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

Events
^^^^^^

.. toctree::
   :maxdepth: 1

   webgc-events-onchange.rst

|

See it in Action
----------------

Try the Sample Richtexts

.. toctree::
   :maxdepth: 1

   ../../gsguide/samples/sample-richtext

|


Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.