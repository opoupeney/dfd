.. image:: ../../images/badges/badge_mobile.png
   :class: pull-right

Image
=====

The image control is used to display images. An image is specified with a url. Images can be from external or
internal sources. Internal sources can be imported using the Resources option in System Configuration & Settings in the
DreamFace Studio to add an image as a resource.

|

.. image:: ../../images/gcs/mob/mobgc-image.png

|

The Image control properties can be set for the following property categories:

* :ref:`mobgc-image-main-label`
* :ref:`mobgc-image-styling-label`
* :ref:`mobgc-image-events-label`

|

.. _mobgc-image-main-label:

Main Properties
---------------

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Main Properties**    | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Name                   | imgImage#         | Name is a reference to the component's DOM element. It can be used to dynamically access   |
|                        |                   | and set component properties. DreamFace gives a default name of *imgImage1* where #        |
|                        |                   | corresponds to the order in which the control was created. The second image created will   |
|                        |                   | have a default Name of *imgImage2*. Name is not required and can be removed if not needed. |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Source                 | Any text          | The source of the image.                                                                   |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Display                | *true* or *false* | The value can either be a literal *true* to display the field or *false* to hide it, or it |
|                        | angular expression| be a angular expression that evaulates to *true* or *false*, for example,                  |
|                        |                   |                                                                                            |
|                        |                   | 5 > 2 would evaluate to *true* and 5 < 2 would evaluate to false.                          |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|
|

.. _mobgc-image-styling-label:

Styling Attributes
------------------

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Styling Attributes** | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Style                  | CSS syles         | CSS style attribure(s) to use for this component, separated by semi-colons, for example:   |
|                        |                   | *color:red; background-color:lightgray*.                                                   |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Classes                | CSS class         | Name of CSS class to use for the component.                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Dynamic Classes        | CSS Class         | The Dynamic Class is a CSS class that will be added to the graphical control if an Angular |
|                        |                   | Expression is verified. It is rendered as a ng-class attribute.                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Width                  | number of pixels  | The width of the image in pixels, for example 150px, which is the default value.           |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Height                 | number of pixels  |The height of the image in pixels, for example 150px, which is the default value.           |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

.. _mobgc-image-events-label:

.. include:: mobgc-props-events.rst

Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.

|

