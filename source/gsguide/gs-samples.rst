.. _samples-label:

Exploring the Samples Gallery
=============================

|

Downloading Samples from Github
-------------------------------

The samples contained in the Samples Gallery are available for download directly from the DreamFace Studio.

.. toctree::
   :maxdepth: 1

   ../../../gsguide/samples/samples-download-from-github

|

Sample GCs
----------

Basic
^^^^^

These samples show Best Use Cases for the Basic graphical controls :

.. toctree::
   :maxdepth: 1

   ../gsguide/samples/sample-statictext
   ../gsguide/samples/sample-buttons
   ../gsguide/samples/sample-icons
   ../gsguide/samples/sample-images
   ../gsguide/samples/sample-htmls
   ../gsguide/samples/sample-carousels
   ../gsguide/samples/sample-treeviews

Input
^^^^^

Samples showing best practices for simple graphical controls are associated with one input field :

.. toctree::
   :maxdepth: 1

   ../gsguide/samples/sample-input
   ../gsguide/samples/sample-textarea
   ../gsguide/samples/sample-datepicker
   ../gsguide/samples/sample-select
   ../gsguide/samples/sample-slider
   ../gsguide/samples/sample-knob
   ../gsguide/samples/sample-chips
   ../gsguide/samples/sample-rating
   ../gsguide/samples/sample-richtexts
   ../gsguide/samples/sample-progressbars


Menu
^^^^

Samples showing best practices for Menu controls are graphical controls that are used to create different types of menus :

.. toctree::
   :maxdepth: 1

   ../gsguide/samples/sample-fab
   ../gsguide/samples/sample-iconbar
   ../gsguide/samples/sample-treemenu
   ../gsguide/samples/sample-hzmenu


Selection
^^^^^^^^^

Sample Best practices for selection graphical controls :

.. toctree::
   :maxdepth: 1

   ../gsguide/samples/sample-radio
   ../gsguide/samples/sample-checkbox
   ../gsguide/samples/sample-switch

|


Sample Tables
^^^^^^^^^^^^^

Table controls are used to present and manage the presentation of information in table format of rows and columns. Below
is a description of the Table graphcical controls available for building web applications in the View Editor:

.. toctree::
   :maxdepth: 1

   ../gsguide/samples/sample-datatable

|

Sample Charts
^^^^^^^^^^^^^

.. toctree::
   :maxdepth: 1

   ../gsguide/samples/sample-barchart
   ../gsguide/samples/sample-hzbarchart
   ../gsguide/samples/sample-piechart
   ../gsguide/samples/sample-donutchart
   ../gsguide/samples/sample-linechart
   ../gsguide/samples/sample-cmlinechart
   ../gsguide/samples/sample-areachart

|

Layout
^^^^^^

Layout is a special graphical control that are containers for other controls. The container is organized in a layout of
rows and columns where other graphical controls can be added to create the user interface. Below is a description the Layout
graphcical controls available for building web applications in the View Editor:

.. toctree::
   :maxdepth: 1

   ../gsguide/samples/sample-panel
   ../gsguide/samples/sample-tabs
   ../gsguide/samples/sample-wizard

|

Other Samples
^^^^^^^^^^^^^

.. toctree::
   :maxdepth: 1

   ../gsguide/samples/sample-crud

|

Dynamics Samples
^^^^^^^^^^^^^^^^

Resources
^^^^^^^^^

CRUD / wMiniCrudModal

JSLibraries / wjavascriptResource
DynamicAccordion / wDynamicAccord

DynamicAdd / wDynamicContainersAdd
SparkLineGrid / wSampleGrid
GridImages / wGridImagesUrl
gridFilters / wGridFilters

GridStyling / wGridCellClasses + wGrid
StaticFormValidation / wFormsValidation + wFormsValidation2
CheckBoxToggle / CheckBocToggle
PanelInPanel / wDynamicPanelInPanel

|

API Services
============

APIChaining / wTwitterMode1

APICharts / wUsaPopulationStatistics + wChartFilter (became wFilterChart)
HomePage / wDFHomePage

DynamicTab / wTabsMovies

FlexDisp / wFlexCss
WeatherForecast / wWeatherHorizon
DFGrids / wGridStyles
PubSub / wPublisher + wSubscriber
GridHTML / wGridMoviesHtml

FlightStat / wAirportFlights
GoogleMaps / wGoogle

Carousel / wEmpCarousel
sSelCandidate / wModernLayout
ModifyingCharts / wModifyingCharts

CRUD / wMiniCrudModal

DynamicPanel / wPanelDynamic
Tree/ <empty>
DynamicList / <empty>
TodoList / wTodoSimple
AlertBoxes / wAlertDirectiveAutoHide
RadioToggle / <empty>
Home / wDFHomePage
DynamicClass / wTabsDynamicClasses + wAccordionDynamicClass







UIElements

wBadgesAndLabels
	- Shows how to use the variety of classes available in the style sheet to highlight labels
	- Note the use of an HTML element in the grid to which we apply the class
	- Note the use of the “jumbotron” class for the title column class


wButtons
	- Shows samples of the various default buttons styles and how to change the styles dynamically
	- Note how to use the {{combobox_value_model}} to change the component/class
	- Note how to use a JS expression in “dynamic Class” property of the button

wComboBox
	- Shows hoe Combo Box can be linked to Model variables
	- Show how to manipulate Models in JS and how immediately the Model replicates the effect to the GC
	- Note: how to link com box to a structured JSON (the model) and how to determine the model value that represents the selection
	- Note how to manipulate the JSON/Model in JS and the immediate effect on the rendering of the GC

wInputBox
	- Shows how to leverage Models to affect size, color, label, label positions, etc. of GC (in this case Input Text)
	- Note: the usage of Model variables ({{myModelVariable}}) in properties like “label”, “width” of a component, “Custom CSS” of a component , etc.


wComboBoxSurvey
	- Creating a dynamic survey from a JSON stream. the survey would have questions (titles) and choices of answers, rendered as combo boxes, with the results captured dynamically in the model.
	- This example shows many things at the same time:
		- How to use JSON to render Comboboxes dynamically (combo put in a recurring panel and we use the “item” dynamic iterator to get all instances of the JSON file)
		- How to use dynamic classes to change the presentation: the radio buttons that determine the layout (2 columns, 3 columns, etc) have a “value” of “col-md-4”, etc.. At the same time, the panel where combos are rendered has its class defined as “{{style_model}}” that changes with the choice of the combo
		- How to add a record or delete a record to the model (see addSurvey and delete survey functions). Note that these functions, when called, are using the parameter $index that is set automatically to refer to the current “instance” where the action is taking place
	- In particular look at:
		- data binding of the combo box
			- item.title: iterator on the title
			- item.choices: so every combo content is the item instance of “choices” array that corresponds to the iterator value
			- Value of the combo box: survey[$index].value to put the chosen value of the combo in the right placeholder of the model
		- Dynamic class: look at the dynamic panel body CSS that contains the combo. We used a custom style class (look at Styles) to float left and “col-md-12” to have it by default to be 1 column rendering
		- The “Show Results” tab shows the selected values for all the combos by iterating over the survey.value values
		- The “scissors” icon: it is a static text where its class is using the Dont awesome class (fa fa-cut fa-2x - refer to Font Awesome to use virtually any of the supported classes)

wImageChange
	- Shows how you can change the attributes of an HTML element by using sliders and knobs linked (by model) to the HTML properties and attributes. The example shows the same techniques applied to a standard GC (round button) and demonstrates how you can change the background color properties
	- Note in particular:
		- The image HTML tag that includes Angular dependencies (in the form of {{myScopeVariable}}) that is set by the various GC used
		- In the case of the button, we used the “Custom CSS” properties of the button and we used the Angular expressions to make the change. Note that this could’ve been done by changing the class or the dynamic class or any other attribute of the button

wRating GC
	- Shows different usage scenarios of the rating GC (various attributes settings, data binding, etc.)
	- Note:
		-the use of an expression in the “Static text” to mean “High/Medium/Low” when the value of the rating is at a level or another
		- Rating object can have a different number of images representing a configurable range of values (for example 10 stars to show a value from 0-50), with configurable steps



GCExtended
==========

wProgressBarGC
	- Shows how to add a custom Angular Directive to the palette of available GC and how to make it interact with other GC in the widget
	- Look in particular to the customer Directive code in the “script” section and to the progressBar GC in the HTML element
	- QUESTIONS: WHY the HTML IS AS-IS? some values are indicated as “val1” whereas others as {{unit_mdl}}
	- QUESTIONS: HOW CAN WE MAKE THIS DIRECTIVE REUSABLE ACROSS THE WHOLE APP? WHERE DO WE PUT THE CODE? HOW CAN WE “ADD IT TO THE GC LIBRARY”

wAlertDirective
	- This widget shows the usage of Angular directives and ng-repeat to create a custom presentation. An alert box is created as an Angular directive, then used by an HTML element that uses ng-repeat to render the directive x-times based on a $scope variable defined in DF
	- Note
		- The Directive code and how it is defined to take parameters
		- The HTML object code that is using the directive and binding the DF functions and model values to feed the directive

FORMS
======

wFormsValidation
	- Sample login screen that demonstrates the usage of Angular form properties to enable/disable buttons and actions as well as to change some look and feel of some gC
	- This example uses some interesting techniques to copy an object to another, reset forms simply, uses the $pristine and $error.required angular context to manage the form
	- Note
		- The “disabled” proper of the button is an expression that uses $error.required (all fields are required)
		- the password buttons need to be 6-10 characters (as per their properties setup).
		- the Static text above the button shows how the content and class can change dynamically (Angular expression) by using label as an expression and the same for the “dynamic class”
		- The usage of the $setpristine() function and the copy of angular objects to enable a coherent reset functionality
		- The button is using the main Form validation. It can use the “panel form” as well if we want to be more precise (so each panel can have its own form, controller, etc. and can be used as a separate scope)

|

Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.
