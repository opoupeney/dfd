View Editor ToolBar
===================

Description
^^^^^^^^^^^

ToolBars are defined in container Graphical Controls such as: Panel, Row-Layout, Column-Layout. Toolbars have a pre-define
structure composed of 3 elements:

* Left Menu
* Title
* Right Menu

The toolbar is displayed based on the evaluation of an angular expression.


Left Menu
---------
The left menu is displayed as an icon with a cascading menu for its children. DEPENDING ON THE MENU “STYLE”, THIS CAN BE ONE ICON SHOWING, 2 ICONS or more, LABEL LINK MENU… Said differently, on the left side, we take a MENU GC (should be able to select from menu GC styles we have) and let the menu style dictates what goes there
SAME COMMENT FOR THE RIGHT MENU


The left menu can be displayed according to an angular expression.


Title
-----

The title can be either an angular expression displaying a value using the default toolbar title’s style from Angular Material. It can also be an html content in which scope variables can be used.
The title menu can be displayed according to an angular expression.
Right Menu
The right menu is displayed as:


Icon + cascading menu
Icon Bar
links (later version)
buttons (later version)
fab (later version)


I THINK WE CAN JUST DEFINE IT AS A MENU GC AND CHOOSE A STYLE. ONE OF THE STYLES CAN BE FAB, BUTTON, etc. the list can grow with time adding different choices


The right menu can be displayed according to an angular expression.


Toolbar Styles


Because toolbars may overload the look when they are into column layout (too much blue backgrounds for example) it must be easy to change the style, and specially the colors, of toolbars.
Designer
A generic directive must be used to set toolbar options. This directive will be added to all component that can have a toolbar


