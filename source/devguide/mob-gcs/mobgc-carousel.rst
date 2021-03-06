.. image:: ../../images/badges/badge_mobile.png
   :class: pull-right

Carousel
========

A Carousel is a graphical component that lets you scroll easily through a set of images.

|

.. image:: ../../images/gcs/mob/mobgc-carousel.png

|

The Carousel control properties can be set for the following property categories:

* :ref:`mobgc-carousel-main-label`
* :ref:`mobgc-carousel_options-label`
* :ref:`mobgc-carousel-styling-label`
* :ref:`mobgc-carousel-events-label`

|

.. _mobgc-carousel-main-label:

Main Properties
---------------

|

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Main Properties**    | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Id                     | nnnnn             | Id is a unique identifier that is 5 or more digits long. It is generated by DreamFace and  |
|                        |                   | can be used when refering to this field in script.                                         |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Name                   | crsCarousel#      | Name is a reference to the component's DOM element. It can be used to dynamically access   |
|                        |                   | and set component properties. DreamFace gives a default name of *crsCarousel#* where #     |
|                        |                   | corresponds to the order in which the control was created. The second button created       |
|                        |                   | will have a default Name of *crsCarousel2*. Name is not required and can be removed if not |
|                        |                   | needed.                                                                                    |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Auto Size              | *true* or *false* | *true* to auto-size the display and *false* to display based on defined size.              |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Display                | *true* or *false* | The value can either be a literal *true* to display the field or *false* to hide it, or it |
|                        | angular expression| be a angular expression that evaulates to *true* or *false*, for example,                  |
|                        |                   |                                                                                            |
|                        |                   | 5 > 2 would evaluate to *true* and 5 < 2 would evaluate to false                           |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

.. _mobgc-carousel_options-label:

Options Items
----------


+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Menu Items**         | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Static                 | Editor            | Beside the Static menu property is a **Edit** link to the Menu Editor. You define the Menu |
|                        |                   | in the Menu Editor. Once you are satisfied you save the menu that has been defined.        |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Dynamic                | Name              | This field takes the name of a Dynamic Menu                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

.. _mobgc-carousel-styling-label:


Styling Attributes
------------------

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Styling Attributes** | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Width                  | number in pixels  | This number represents the width of the carousel in the row of the panel in %. The default |
|                        |                   | is 100% of the row, column where it is displayed in the panel.                             |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Max Width              | number in pixels  | This number represents the maximum width of the carousel in pixels. The default value is   |
|                        |                   | 1200.                                                                                      |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Max Width              | number in pixels  | This number represents the maximum height of the carousel in pixels. The default value is  |
|                        |                   | 600.                                                                                       |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Style                  | CSS syles         | CSS style attribure(s) to use for this component, separated by semi-colons, for example:   |
|                        |                   | *color:red; background-color:lightgray*. By clicking on the **...** on the right hand side |
|                        |                   | of the field, a window opens up proposing to change attributes for **font**, **color**,    |
|                        |                   | **padding** and **margin** presented in a tree. When clicking on the arrow to the left of  |
|                        |                   | the attribute type, the user is guide by placeholder to enter the correct settings         |
|                        |                   |                                                                                            |
|                        |                   |        .. image:: ../../images/gcs/dfx-icon-css.png                                        |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Classes                | CSS class         | Name of CSS class to use for the component.                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Dynamic Classes        | CSS Class         | The Dynamic Class is a CSS class that will be added to the graphical control if an Angular |
|                        |                   | Expression is verified. It is rendered as a ng-class attribute.                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

.. _mobgc-carousel-events-label:

.. include:: mobgc-props-events-focus.rst

Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.

|

