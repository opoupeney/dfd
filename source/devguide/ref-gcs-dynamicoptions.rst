Dynamic Options
===============


Dynamic Options allow us to create Graphical Controls based on different (or any) names of objects properties.

Dynamic Objects are used in many :term:`GC`s. There are two types of Dynamic Options:

*Options used in GCs:

   * Carousel
   * Select
   * Slider
   * RadioButton
   * Checkbox
   * Switch

* Options used in Menu Items:

   * Button
   * Fab
   * HorizontallMenu
   * Iconbar
   * TreeMenu


Carousel Options
^^^^^^^^^^^^^^^

Source - name of scope array with objects for Carousel GC (required).
Title - name of Source object property that contain Carousel title (not required).
Description - name of Source object property that contain Carousel Description (not required).
Image Src - name of Source object property that contain Carousel item picture link (required).
Action - name of Source object property that contain Carousel item onclick event (not required).

::

$scope.myCarousel = [{
   "landscape": "<h4>Forest</h4>",
   "country": "<h2>Costa Rica</h2>",
   "photo": "'https://www.travelexcellence.com/images/movil/La_Paz_Waterfall.jpg'",
   "action": "myFunction()"
}];



Checkbox Options
^^^^^^^^^^^^^^^
Source - name of scope array with objects for Checkbox GC (required).
Checked Value - name of Source object property when Checkbox is checked (required).
Unchecked Value - name of Source object property when Checkbox is unchecked (required).
Label - name of Source object property that contain Checkbox label (not required).


::

$scope.myCheckbox = [{"isSubscribe":"Subscribe to newsletter?", "posAnswer":true, "negAnswer":false}].



RadioButton Options
^^^^^^^^^^^^^^^^^^^

Source - name of scope array with objects for RadioButton GC (required).
Value - name of Source object property with RadioButton value (required).
Label - name of Source object property that contain RadioButton label (not required).


Example:

::

   $scope.myFruits = [{"code": 1, "name": "Apple"}, {"code": 2, "name": "Banana"}, {"code": 3, "name": "Kiwi"}];


Select Options: the same as with RadioButtons.
Slider Options: the same as with RadioButtons.
Switch Options: the same as with Checkbox.


Dynamic Options for GCs with Menu Items.


There three types of Menu Items Dynamic Options:


* Main ( Main Properties tab inside Menu Editor Dynamic Options section);
* State ( State Properties tab ). Available only for singe Iconbar GC and for Iconbar in Toolbar;
* Wait ( Wait Properties tab ). Available only for root level Buttons Menu of singe Button GC and Toolbar Buttons.


Main Properties:


Source - name of scope array with Menu Item objects (required).
Type - name of Source object property that contain Menu Item type name (not required). Type can be one of three: ‘standard’, ‘title’, ‘divider’. If there is no Type property in Menu Item object - Menu Item will be created as ‘standard’.
Label - name of Source object property that contain Menu Item label (not required).
Icon Object Name - name of Source object property that contain Menu Item icon object name (not required). But If is set it is necessary to set Icon Name and Icon Type.
Icon Name - name of Source object property that contain Menu Item icon name (required if Icon Object Name is set).
Icon Type - name of Source object property that contain Menu Item icon type (required if Icon Object Name and Icon Name are set).
Shortcut - name of Source object property that contain Menu Item shortcut (not required).
Notification - name of Source object property that contain Menu Item notification value (not required).
Display - name of Source object property that contain Menu Item display (not required).
Disabled - name of Source object property that contain Menu Item disabled (not required).
Action - name of Source object property that contain Menu Item onclick event (not required).
Children Items - name of Source object property that contain name of Children menu items array (not required).


State Properties:


State Object Name - name of Source object property that contain Menu Item State object name (not required).
Binding - name of Source object State object property that contain Menu Item State object binding name (not required).
Checked/Unchecked Icon Object Name - name of Source object State object property that contain Menu Item State object checked/unchecked icon object name (not required). But If is set it is necessary to set Icon Name and Icon Type.
Checked/Unchecked Icon Name - name of Source object State object property that contain Menu Item State object checked/unchecked icon name (required if Icon Object Name is set).
Checked/Unchecked Icon Type - name of Source object State object property that contain Menu Item State object checked/unchecked icon type (required if Icon Object Name and Icon Name are set).
Checked/Unchecked Icon Style - name of Source object State object property that contain Menu Item State object checked/unchecked icon style (not required).
Checked/Unchecked Icon Class - name of Source object State object property that contain Menu Item State object checked/unchecked icon class (not required).






Wait Properties:
Wait Object Name - name of Source object property that contain Menu Item Wait object name (not required).
Binding - name of Source object Wait object property that contain Menu Item Wait object binding name (not required).
AutoDisabled - name of Source object Wait object property that contain Menu Item Wait object autoDisabled name (not required).
Icon Object Name - name of Source object Wait object property that contain Menu Item Wait object icon object name (not required). But If is set it is necessary to set Icon Name and Icon Type.
Icon Name - name of Source object Wait object property that contain Menu Item Wait object icon name (required if Icon Object Name is set).
Icon Type - name of Source object Wait object property that contain Menu Item Wait object icon type (required if Icon Object Name and Icon Name are set).
Icon Style - name of Source object Wait object property that contain Menu Item Wait object icon style (not required).
Icon Class - name of Source object Wait object property that contain Menu Item Wait object icon class (not required).






Examples of most complex GCs with Menu


Iconbar

::
$scope.myIconbar = [
      {
      	"myIconbarLabel": "'My first root Item'",
        	"myIconbarIcon": {
"myIconbarIconName": "'star'",
"myIconbarIconType": "svg-icon"
},
       	"myIconbarType": "standard",
        	"myIconbarShortcut": "",
       	"myIconbarNotification": "",
       	"myIconbarDisplay": "true",
        	"myIconbarDisabled": "false",
        	"myIconbarOnclick": "",
        	"myIconbarItems": [
          		{
            		"myIconbarLabel": "'My Iconbar Item'",
            		"myIconbarIcon": {
"myIconbarIconName": "'apple'",
"myIconbarIconType": "svg-icon"
},
            "myIconbarType": "standard",
            		"myIconbarShortcut": "",
            "myIconbarNotification": "",
            "myIconbarDisplay": "true",
            "myIconbarDisabled": "false",
            "myIconbarOnclick": "",
            "myIconbarItems": [
            			{
                  				"myIconbarLabel": "'My Iconbar Item'",
                  				"myIconbarIcon": {
"myIconbarIconName": "'apple'",
"myIconbarIconType": "svg-icon"
},
            "myIconbarType": "title",
            "myIconbarShortcut": "",
            "myIconbarNotification": "8",
            "myIconbarDisplay": "true",
            "myIconbarDisabled": "false",
            "myIconbarOnclick": "toggleScopeState()",
            "myIconbarItems": [],
                  				"myState": {
                      					"myStateBinding": "scopeState",
                      					"myStateCheckedIcon":   {
"myStateIconName": "'thumb_up'",
 "myStateIconType": "svg-icon",
 "myStateIconStyle": "color:lightgreen",
 "myStateIconClass": "greened"
},
                      "myStateUncheckedIcon": {
"myStateIconName": "'thumb_down'",
 "myStateIconType": "svg-icon",
 "myStateIconStyle": "color:violet",
 "myStateIconClass": "violetted"
}
                  				}
                			}
            		],
            		"myState": {
                			"myStateBinding": "scopeState",
            "myStateCheckedIcon":   {
"myStateIconName": "'thumb_up'",
"myStateIconType": "svg-icon",
"myStateIconStyle": "color:lightgreen",
 "myStateIconClass": "greened"
},
            "myStateUncheckedIcon": {
"myStateIconName": "'thumb_down'",
 "myStateIconType": "svg-icon",
 "myStateIconStyle": "color:violet",
 "myStateIconClass": "violetted" }
            			}
          			},
          			{
            "myIconbarLabel": "'My Iconbar Item'",
            "myIconbarIcon": {
"myIconbarIconName": "'free_breakfast'",
 "myIconbarIconType": "svg-icon"
},
            "myIconbarType": "divider",
            "myIconbarShortcut": "",
            "myIconbarNotification": "7",
            "myIconbarDisplay": "true",
            "myIconbarDisabled": "false",
            "myIconbarOnclick": "",
            "myIconbarItems": []
          			}
        		]
      },
      {
      		"myIconbarLabel": "'My second root Item'",
"myIconbarIcon": {
"myIconbarIconName": "'stars'",
"myIconbarIconType": "svg-icon"
},
           "myIconbarType": "standard",
           "myIconbarShortcut": "",
           "myIconbarNotification": "",
           "myIconbarDisplay": "true",
           "myIconbarDisabled": "false",
           "myIconbarOnclick": "",
           "myIconbarItems": [],
           "myState": {
        			"myStateBinding": "scopeState",
          	"myStateCheckedIcon":   {
"myStateIconName": "'thumb_up'",
"myStateIconType": "svg-icon",
"myStateIconStyle": "color:lightgreen",
"myStateIconClass": "greened"
},
     	     	"myStateUncheckedIcon": {
"myStateIconName": "'thumb_down'",
"myStateIconType": "svg-icon",
"myStateIconStyle": "color:violet",
"myStateIconClass": "violetted"
}
        		}
      	}
];


After we must connect those properties to Iconbar (for example in left side of Panel Toolbar) like on screen:






















for main Iconbar Properties:

for State Iconbar Properties:









Buttons:

::
$scope.myButtons = [
      	{
      		"myButtonsLabel": "'My Button Label'",
       	 "myButtonsIcon": {
"myButtonsIconName": "'star'",
"myButtonsIconType": "svg-icon"
},
       	"myIconbarType": "standard",
        		"myButtonsShortcut": "123",
        	"myButtonsNotification": "5",
        		"myButtonsDisplay": "true",
"myButtonsDisabled": "false",
            "myButtonsOnclick": "toggleScopeState()",
            "myButtonsItems": [],
            "myWait": {
            "myWaitBinding": "scopeState",
            "myWaitAutoDisabled": "scopeState",
            "myWaitIcon": {
                "myWaitIconName": "'fa-spinner'",
                "myWaitIconType": "fa-icon",
                "myWaitIconStyle": "",
                "myWaitIconClass": "fa-pulse"
            		}
        }
      },
      {
        "myButtonsLabel": "'My Button Label'",
        "myButtonsIcon": {
"myButtonsIconName": "'stars'",
"myButtonsIconType": "svg-icon"
        },
        "myButtonsType": "standard",
        "myButtonsShortcut": "",
        "myButtonsNotification": "",
        "myButtonsDisplay": "true",
        "myButtonsDisabled": "false",
        "myButtonsOnclick": "toggleScopeState()",
        "myButtonsItems": [
        			{
              "myButtonsLabel": "'My Button Label'",
              "myButtonsType": "title"
            },
          			{
              "myButtonsType": "divider",
            }
        		]
      	}
];


Connecting Main Properties (for example in right side of Panel Toolbar):



Connecting Wait Properties:

Fab:
lets connect $scope.myButtons to our Fab (simple Fab GC):
And lets create in scope state variable and toggle function for it:

::
$scope.scopeState = false;

	$scope.toggleScopeState = function() {
		$scope.scopeState ? $scope.scopeState = false : $scope.scopeState = true;
	};
As a result - all three components created using dynamic options from scope and connected to scope and ‘see’ scope changes.



+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| **Options Items**      | Possible Values   | Description                                                                                |
+========================+===================+============================================================================================+
| Static                 | Defined in Slide  | Beside the Static menu property is an **Edit** link to the Slied Editor. Here you can      |
|                        | Editor            | you define the slides that will be displayed using an editor to guide the definition.      |
|                        |                   | Once you are satisfied you save the menu that has been defined.                            |
|                        |                   |                                                                                            |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+
| Dynamic                | Name              | This field takes the name of a Dynamic Menu                                                |
+------------------------+-------------------+--------------------------------------------------------------------------------------------+

