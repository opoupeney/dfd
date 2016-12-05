Sample Statictext
=================

A Page with a full range of Text controls is provided below in the Samples Application. By visiting the Sample Text
page you can test the functionality and play with the sample Statictext controls. By importing this page from the Github
Samples repository you will be able to use the samples in your applications.

* `Try Sample Staticexts <http://50.22.58.40:3300/deploy/qa/Samples/web/1.0.1/index.html#/page.html?login=guest&name=SampleTexts>`_
* :ref:`samples-github-label`

|

Sample Categories - different kinds of Statictext controls are provided as examples:

|

Basics
------

This is a basic Statictext example with just the label changed.

.. image:: ../../images/devguide/samples/sample-text-basics.png

|

Styles
------

The Styles examples show three types of styles

* Custom styles added directly in the Styles property
* An example uses a CSS Class defined in the Styles Editor of DreamFace
* An example of a Dynamic CSS Class that is invoked by the Click event

.. image:: ../../images/devguide/samples/sample-text-styles.png

The first example sets a custom style with CSS added in the Style property.

Style: *font-family:Bungee;font-size:28px;color:#b91caf;*

The second sample uses a CSS Class **changeTextStyle** defined in the Styles editor:

::

    .codechangeTextStyle {
        font-family: "Comic Sans MS";
        border: 2px solid #29a4ff;
        padding: 5px;
        background-color: #a6f1ff !important;
        font-style: italic;
    }

The third example uses a Dynamic Class that is defined in the Styles Editor and a function that is invoked by the Click
event. When the text is clicked the text toggles to red color and when clicked again it toggles back. The function is
defined in the Script Editor.

To achieve this we need to

1. set up a dynamic CSS Class, in our sample **changeTypeColor**

::

    ..changeTypeColor{
	    color:red !important;
    }

2. Create a function to toggle the value of **changeTextColor** boolean variable to *true* in the DreamFace Script Editor.

::

   /*change color text dynamic Style*/
   $scope.changeText = function(){
      $scope.changeTextColor = !$scope.changeTextColor;
   };

3. Add the function to the OnClick event and test change the Dyanamic Class propery to test the value of the
**changeTextColor** variable and if true to execute the Dynamic CSS Class to change the color of the text to red.

OnClick: *changeText()*

Dynamic Class: *{changeTypeColor:changeTextColor}*

|


Bindings
----------------

Binding samples show two examples of bindins:

* A simple binding with a scope variable
* A more complex binding using an angular express.

.. image:: ../../images/devguide/samples/sample-text-bindings.png

1. In the first example we set the Text property to the scope variable **sampleBindVar**. The scope variable is set in the
Script with the Script Editor.

::

    /*simple binding*/
    $scope.sampleBindVar = "Simple binding with a scope variable";

2. In the second example define the value of the scope variable **sampleBindVar**.

::

    /*complex binding*/
    $scope.sampleBindVarExp = "Complex binding with an expression";

Set the Text property to the desired angular expression.

Text: *'Binding: '+ sampleBindVarExp*

|


Events
------

The sample events show how to show text or hide it on mouse-enter, mouse-leave and click events.

.. image:: ../../images/devguide/samples/sample-text-events.png

Define the functions you will use in the script editor:

::

   /*show text when mouse leave*/
   $scope.showTextOnMouseLeave = function(){
  	   $scope.showTextOnMouseLeaveBoolean = true;
       $scope.showTextOnMouseEnterBoolean = false;
   };

   /*show text when mouse enter*/
   $scope.showTextOnMouseEnter = function(){
  	   $scope.showTextOnMouseEnterBoolean = true;
       $scope.showTextOnMouseLeaveBoolean = false
   };

   /*hide text on click*/
   $scope.hideTextOnClick = function(){
       $scope.showTextOnMouseEnterBoolean = false;
       $scope.showTextOnMouseLeaveBoolean = false;
   };

   /*show text when mouse over*/
   $scope.showTextOnMouseOver = function(){
   	   $scope.showTextOnMouseOverBoolean = true;
   };

    /*hide text when mouse leave*/
    $scope.hideTextOnMouseLeave = function(){
  	   $scope.showTextOnMouseOverBoolean = false;
       $scope.showTextOnClickBoolean = false;
     };

For the first example set the set the following events which will hide text in the center when clicked and shows a
message on Mouse Enter and Leave events by changing Display option on the text fields to show or hide.

OnClick: *hideTextOnClick()*

OnMouseEnter: *showTextOnMouseEnter()*

OnMouseLeave: *showTextOnMouseEnter()*

|

For the second example set the set the following events which will set the text in the center to *You clicked* when
clicked and shows a message on Mouse Enter and Leave events.

OnClick: *showTextOnClick()*

OnMouseEnter: *showTextOnMouseOver()*

OnMouseLeave: *hideTextOnMouseLeave()*


|

