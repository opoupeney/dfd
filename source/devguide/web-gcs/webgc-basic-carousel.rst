.. image:: ../../images/badges/badge_web.png
   :class: pull-right

Carousel
========

.. image:: ../../images/icons/basic_carousel.png
    :width: 50px
    :height: 50px

A Carousel is a graphical component that lets you scroll easily through a set of images or slides.

|

.. image:: ../../images/gcs/web/webgc-carousel.png
   :width: 500px

|

See it in Action
----------------

Try the Sample Carousel controls

.. toctree::
   :maxdepth: 1

   ../../gsguide/samples/sample-carousels

|

Reference
---------

The Carousel control properties can be set for the following property categories:

Button Main Properties allow us to set the Button Label, Icon, Menu Items if the Button has a menu and whether the Button
is displayed and enabled.

.. toctree::
   :maxdepth: 1

   webgc-prop-main-id
   webgc-prop-main-template
   webgc-prop-main-name
   webgc-prop-main-autoslide
   webgc-prop-main-display
   webgc-prop-main-options

|

Styling Attributes
^^^^^^^^^^^^^^^^^^

.. toctree::
   :maxdepth: 1

   webgc-prop-style-flexwidth
   webgc-prop-style-maxwidth
   webgc-prop-style-maxheight
   webgc-prop-style-style
   webgc-prop-style-class
   webgc-prop-style-dynamic


Carousel Quickstart
^^^^^^^^^^^^^^^^^^

In summary the Carousel has 5 properties itself and each slide (or Carousel option) has 5 properties:

The Carousel properties are :

* Options source (array). Can be static/dynamic. For static representation that array can be defined in the . For dynamic - need to put scope array name into field ‘Dynamic’ of Options section in Property panel.
* Autoplay (boolean). By default ‘false’.
* Slide Interval (millisecond). Dy default 3000.
* Max Width a number in pixels. The default is ‘1200px’.
* Max Height- a number in pixels. The default is ‘400px’.

**Note** Max Width and Max Height needs to be set for responsive design for calculating proportion sides of the Carousel.

Carousel Slide option properties:

Name - it is parameter for accessibility in static representation inside popup dialog (no need to set it in dynamic represenation).
Src - is the image url. In static representation it is expression. It is possible to put into src field image url without/within quotes and as a scope variable (like that 'src': 'scopeSrc'). In dynamic - it is just real image url.
Title - html content inside which it is possible to use scope variables. For static representation in popup dialog click ‘Edit’ button to open ‘Html Editor’ and edit it.
Description - the same as ‘Title’.
Onclick - is ‘ng-click’ event on Slide image.

A Slide Editor is avaiable to define the Slides and Slide options, to add or remove slides and to change the order of the slides.


Example
'''''''

Default static representation (pre-defined by default in the Slide Editor): ::

    "static": { "value": [
            {
              "name": "slide1",
              "title": "<h2>Sample Title 1</h2>",
              "description": "<h4>Sample Description 1</h4>",
              "src": "'https://www.travelexcellence.com/images/movil/La_Paz_Waterfall.jpg'",
              "onclick": ""
            },
            {
              "name": "slide2",
              "title": "<h2>Sample Title 2</h2>",
              "description": "<h4>Sample Description 2</h4>",
              "src": "'http://images.kuoni.co.uk/73/indonesia-34834203-1451484722-ImageGalleryLightbox.jpg'",
              "onclick": ""
            },
            {
              "name": "slide3",
              "title": "<h2>Sample Title 3</h2>",
              "description": "<h4>Sample Description 3</h4>",
              "src": "'https://www.travcoa.com/sites/default/files/styles/flexslider_full/public/tours/images/imperialvietnam-halong-bay-14214576.jpg'",
              "onclick": ""
    }]}



Example of dynamic representation (add this to the script of the View): ::

    $scope.carouselData = [
          {
            'src': '/_shared/assets/blue-abstract-background.jpg',
            'title': '<h2>{{myTitle}}</h2>',
            'description': '<h4>{{myDescription}}</h4>',
            'onclick': 'myFunction()
          },
        {
            'src': '/_shared/assets/login_logo.png',
            'title': '<h2>Slide Title 2</h2>',
            'description': '<h4>Slide Description <i>{{someVar}}</i></h4>',
            'onclick': 'otherFunction()'
        },
        {
            'src': 'scopeSrc',
            'title': '<h2>Title {{page}}</h2>',
            'description': '<h4>Description {{page}}</h4>',
            'onclick': ''
        }
    ];

    Where: ::

    {{myTitle}}, {{myDescription}}, {{someVar}} and {{page}} - are expressions with scope variables;

    myFunction() and otherFunction() - are scope functions.


This way of using scope variables and functions in the Carousel options (slides) is the same for static/dynamic representation.


|



|

Events
^^^^^^

.. toctree::
   :maxdepth: 1

   webgc-events-focus.rst




Tips and Tricks
^^^^^^^^^^^^^^^

# Remember that values entered in the properties fields only take effect after they have been saved.

Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.

|

