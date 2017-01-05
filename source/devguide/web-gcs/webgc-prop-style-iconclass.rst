.. _webgc-prop-style-class-label:


Icon Class
==========

The Icon Class property defines the name of the CSS Class used for styling the icon.

|

**Value:** - Name of CSS class(es) separated by a space used for styling.

|

.. image:: ../../images/devguide/dfx-prop-style-class.png

**Default:** - *None*

**Notes:**

The Class can be defined in the DreamFace Styles Editor (found in the View Editor) or imported / created in a CSS file
in the Resource Editor (found in the Applicaiton configuration parameters).

Styles defined in Style take precedence over the same styles defined in the Class(es). If color is defined as blue in the
Style Property and Red in the Class Property the color will be blue since the Style property takes precedence.

For more on styling :term:`GC`s see :ref:`gcs-styling-label`.

Example of CSS Class Definition

::

    // Change Icon Color Class
    .changeIconColor * {
      color: #0e3bef;
    }

    Class: changeIconColor

|
