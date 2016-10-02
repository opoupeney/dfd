.. image:: ../../images/badges/badge_web.png
   :class: pull-right

Datatable
=========

.. image:: ../../images/icons/table_datatable.png
    :width: 50px
    :height: 50px

The datatable is used to present data coming from a static array or an API call. Each set of data corresponds to an iteration
of the array (or API call) and is presented in a row of the table.

Data tables help users visualize and manipulate large sets of data with sorting and filtering mechanisms and selection and
multi-selection on rows for treatment as a single row or a group of rows.

|

.. image:: ../../images/gcs/web/webgc-datatable.png

|

|

Features
--------
* Feature 1
* Feature 2
* Feature 3
* Feature 4

|

See it in Action
----------------

* `Try some Areachart Samples <http://dfbluemixsrv02.market-interactive-clouds.com/studio/widget/web/Samples/welcome1/index.html>`_
* Download Samples from Github

|

Reference
---------

Table columns have a value and can be rendered as one of the following pre-defined graphical controls:

* **Statictext**
* **Button**
* **HTML**
* **Image**
* **Rating**

|

.. image:: ../../images/gcs/web/webgc-datatable-gcs.png

The Datatable control properties can be set for the following property categories:

* :ref:`webgc-datatable-main-label`
* :ref:`webgc-datatable-columns-label`
* :ref:`webgc-datatable-render-label`
* :ref:`webgc-datatable-styling-label`
* :ref:`webgc-datatable-events-label`

|

.. _webgc-datatable-main-label:

Main Properties
---------------

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Main Properties**    | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Name                   | dtblDatatable#    | Name is a reference to the component's DOM element. It can be used to dynamically access   |
|                        |                   | and set component properties. DreamFace gives a default name of *dtblDatatable#* where #   |
|                        |                   | corresponds to the order in which it was created. If it's the second datatable created it  |
|                        |                   | will have a default Name of *dtblDatatable2*. Name is not required and can be removed if   |
|                        |                   | not needed.                                                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Binding                | $scope variable   | The data table can be bound to a value contained in a $scope variable.                     |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
|Title                   | Any text          | Title of the table, this can either be text in quotes or an                                |
|                        | Angular Expression| :ref:`angular-expression-label`.                                                           |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Title Visible          | checked           | If checked the Title will be visible, unchecked means Title is not visible.                |
|                        | unchecked         |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Paging                 | checked           | If checked the Title will be visible, unchecked means Title is not visible.                |
|                        | unchecked         |                                                                                            |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Display                | *true* or *false* | The value can be a literal **true** to display the component or **false** to hide it. This |
|                        | Angular Expression| value can also be the result of an :ref:`angular-expression-label` that returns a boolean  |
|                        |                   | value of the true or false, *true* meaning it will be visible, *false* meaning it will not |
|                        |                   | be displayed.                                                                              |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Disabled               | *true* or *false* | Disabled takes a *true* or *false* value. *true means that the component is *Disabled* and |
|                        | Angular Expression| the user cannot interact with it. *false* means the the component is not Disabled but      |
|                        |                   | active and the user can interact with it. This value can also be the result of an          |
|                        |                   | :ref:`angular-expression-label` that returns a boolean value of the true or false, *true*  |
|                        |                   | meaning Disabled and *false* meaning it will be active and available.                      |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

.. _webgc-datatable-columns-label:

Columns
-------

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Columns**            | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Selection Mode         | none              | Selection Mode allows the user to select one or more rows to receive some treatment.       |
|                        | single            | Values for Selection Mode can be *none*, *single* or *multi*; none means no selection box  |
|                        | multi             | will be available for checking, single means only one row can be selected at a time and    |
|                        |                   | multi means that multiple rows can be selected for manipulation.                           |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Column                 | column to define  | Click on the down arrow to choose the column for which you would like to define properties.|
|                        |                   |                                                                                            |
|                        |                   |        .. image:: ../../images/gcs/dfx-dt-gcrenderer-col.png                               |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
|   Header               | text              | The header of the column. This is a text defining the column header like *ID*, *Name*, etc.|
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
|   Value                |                   | This is the value. It can be the variable that contains the data returned from an API call.|
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
|   Renderer             | Statictext,       | The column can be rendered as a graphical control. A list of possible controls is provided.|
|                        | Button,           | The default is Statictext.                                                                 |
|                        | HTML,             | After selecting the Renderer you can click on the the three **...** as seen in the image   |
|                        | Image,            | below:                                                                                     |
|                        | Rating            |                                                                                            |
|                        |                   |        .. image:: ../../images/gcs/dfx-dt-gcrenderer2.png                                  |
|                        |                   |                                                                                            |
|                        |                   | This will bring open the Properities window that corresponds to the graphical control      |
|                        |                   | selected for this column of the table. For example, if you selected a Statictext, you would|
|                        |                   | see this at the top of the properties window, indicating that you are defining properties  |
|                        |                   | for a Statictext component for the datatable dtblDatatable1 column called ID.              |
|                        |                   |                                                                                            |
|                        |                   |        .. image:: ../../images/gcs/dfx-dt-gcrendererID.png                                 |
|                        |                   |                                                                                            |
|                        |                   | Define the properties of the column. When finished, to return to the definition of the     |
|                        |                   | just click on the name of the Datatable, in the example above, you would click on          |
|                        |                   | *dtblDatatable1*.                                                                          |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
|   Ascending            | *true* or *false* | The value can be a literal **true** to order the column in ascending order or **false** to |
|                        | Angular Expression| or in descending order. The value can also be the result of an                             |
|                        |                   | :ref:`angular-expression-label` that returns a boolean value of the true or false.         |
|                        |                   |                                                                                            |
|                        |                   | Clicking on the arrow icon next to the column header will toggle the the value between     |
|                        |                   | *true* and *false* and change the icon accordingly.                                        |
|                        |                   |                                                                                            |
|                        |                   |        .. image:: ../../images/gcs/dfx-dt-ascending.png                                    |
|                        |                   |                                                                                            |
|                        |                   |        .. image:: ../../images/gcs/dfx-dt-descending.png                                   |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

.. _webgc-datatable-render-label:

Rendering
^^^^^^^^^

This is the rendering section.

|

.. _webgc-datatable-styling-label:

Styling Attributes
------------------
|

+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Styling Attributes** | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Style                  | CSS syles         | CSS style attribure(s) to use for this component, separated by semi-colons, for example:   |
|                        |                   | *color:red; background-color:lightgray*. The Datatable has a default size of 100%,         |
|                        |                   | width:100%                                                                                 |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Classes                | CSS class         | Name of CSS class to use for the component.                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Dynamic Classes        | CSS Class         | The Dynamic Class is a CSS class that will be added to the graphical control if an Angular |
|                        |                   | Expression is verified. It is rendered as a ng-class attribute.                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

|

.. _webgc-datatable-events-label:

.. include:: webgc-props-events-focus.rst


Example
-------

Datatable Filtering and Selection

Datatables work with scope data. The data must be array of objects. Objects can be created in scope or taken from API Service Objects.
We can create a function to call an API SO from Code Assistant -> API Services. Then we can add the name of the array to
Datatable “Binding” property. Next is to build table columns according to array structure.

Sample of scope Datatable array:

$scope.data = [
{
   "landscape": "Forest",
   "id": 154,
   "country": "Costa Rica",
   "photo": "https://www.travelexcellence.com/images/movil/La_Paz_Waterfall.jpg"
},
{
   "landscape": "Mountains",
   "id": 225,
   "country": "Indonesia",
   "photo": "http://images.kuoni.co.uk/73/indonesia-34834203-1451484722-ImageGalleryLightbox.jpg"
},
{
   "landscape": "Sea",
   "id": 324,
   "country": "Vietnam",
   "photo": "https://www.travcoa.com/sites/default/files/styles/flexslider_full/public/tours/images/imperialvietnam-halong-bay-14214576.jpg?itok=O-q1yr5_"
},
{
   "landscape": "River",
   "id": 270,
   "country": "USA",
   "photo": "http://www.parasholidays.in/blog/wp-content/uploads/2014/05/holiday-tour-packages-for-usa.jpg"
},
{
   "landscape": "Volcano",
   "id": 115,
   "country": "New Zealand",
   "photo": "http://clickker.in/wp-content/uploads/2016/03/new-zealand-fy-8-1-Copy.jpg" }
];

Datatable have new property Filter ( boolean ) which is a checkbox in Property Panel, which adds a Filter to the Datatable
when the property is checked. The Filter works only in Preview mode. It filters table rows in all the properties of each row.

The selection in the Datatable can be bound to scope. We can create an array of numbers in scope and put the name of that
array into the “Selection Binding” field. Each array number is the Datatable row index. So if we create that array:
$scope.selectedData = [ $scope.data[1], $scope.data[3] ];
it means to select (make table row checkboxes checked) second and third rows.

After we can create our own scope functions and manipulate with Datatable data. Example of such function is:

$scope.chooseRows = function() {
	$scope.selectedData = [ $scope.data[0], $scope.data[2], $scope.data[4] ];
     	$scope.dataArray = [];
      	$scope.newData = [];
      	var newSlide = { src: '' };
      	for (var i=0; i<$scope.selectedData.length; i++) {
          $scope.newData.push({ src: $scope.selectedData[i].photo });
            }
      	$scope.dataArray = $scope.newData;
};

Here we selected first and third table rows and created new array newData with images urls:
$scope.newData = [
	{ "src": "https://www.travelexcellence.com/images/movil/La_Paz_Waterfall.jpg" },
	{ "src": "https://www.travcoa.com/sites/default/files/styles/flexslider_full/public/tours/images/imperialvietnam-halong-bay-14214576.jpg?itok=O-q1yr5_" },
	{ “src”: “http://clickker.in/wp-content/uploads/2016/03/new-zealand-fy-8-1-Copy.jpg” }
];

That array have structure which is good for GC Carousel. So we can create Carousel and put dataArray to “Dynamic” Carousel
property. Also we need some element to call our chooseRows() function.



Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.

|
