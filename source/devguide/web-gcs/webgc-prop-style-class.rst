.. _webgc-prop-style-class-label:


Class
=====

The name of the CSS class used to style the :term:`GC`.

|

.. image:: ../../images/devguide/dfx-prop-style-class.png

**Value:** - Name of CSS class(es) separated by a space used for styling.

**Default:** - *None*

**Notes:**

The Class can be defined in the DreamFace :ref:`dfx-editor-styles-label` (found in the View Editor) or imported / created in a CSS file
in the Resource Editor (found in the Applicaiton configuration parameters).

Styles defined in Style take precedence over the same styles defined in the Class(es). If color is defined as blue in the
Style Property and Red in the Class Property the color will be blue since the Style property takes precedence.

For more on styling :term:`GC`s see :ref:`gcs-styling-label`.

Example of CSS Class Definition

::

   Custom Statictext Tooltip Styling Example

   Add class my-tooltip to Tooltip Properties Class field and those styling rules to View Style Editor:

   // tooltip container style
   .my-tooltip-container { background-color: green; }

   // tooltip text style
   .my-tooltip span {
      border: 2px solid red;
  	  margin: 5px;
  	  background-color: blue;
   }

   Class: my-tooltip-container my-tooltip
|
