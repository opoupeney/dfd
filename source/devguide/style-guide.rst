.. _style-label:

Programming Style Guide, Naming Conventions and Shortcut Keys
=============================================================


Conventions in the View Editor
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Scripts - Some ideas for making scripts more readable and less prone to error.
Formatting rules - Formatting rules help to make code readable for humans and ultimately help to reduce syntax errors or at least to help find them more quickly.

Indentation - It is recommended to use four spaces or one tab for each indentation level. This helps to make code more readable:

.. code-block:: js

    if ( new && new.item) {
     for (i = 0; ….) {
        do something else
      }
    }

Semi-Colons

Line length - Lines of script should be limited to 80 characters in length.

Line breaks - Breaking a long line should be done after an operator and the following line should be indented two indentation levels::

ex. functionX (doc, new.item, new.price, new.description, isNewItem, isInStock, “some string description”,
                abcvar, xyzvar);

Blank Lines  - Blank lines should be used to help make script readable. Instead of having a big block of code, you can use blank lines to separate related lines of code from unrelated lines of code. One idea would be to add a blank line before each flow control statement, like if, for, … at the same time, too many blank lines can also create difficult to read code.

**Reserved Words and Symbols**

The $ prefix is used to namespace Angular-provided services. To prevent collisions it's best to avoid naming your
services and models anything that begins with a $ in the scripts.

**Conventions for Jade Widgets**

Naming Conventions - These naming conventions are suggestions for creating more readable code.
Reserved names and System variables
Naming of constants
Naming Variables and Functions - Variable and function names should be as short as possible but still indicate their purpose in the name. Meaningless names like (myVar, foo, temp), reserved or system variable names and seemingly obvious troublesome names like using ‘i’ as a global variable should be avoided.


**Variable and Function Names**

Variable and function names use camel case and begin with a noun, function names begin with a verb.

    var = numSides
    var = productName
    var = firstName
    function setCount (… )
    function getClient (… )

Common convention id for function verb names are as follows:

====  =================
Verb  Returns (usually)
====  =================
can   boolean
has   boolean
is    boolean
get   nonboolean
set   sets a value
====  =================

|

Naming Conventions
^^^^^^^^^^^^^^^^^


DreamFace component names may only contain alphanumeric characters. Numbers are permitted and are generally used when
creating many of the same type of control. Do not use underscores, hyphens, or any other non-alphanumeric characters.
Spaces are not allowed, they will be accepted without errors in some circumstances but will ultimately cause problems.

Within DreamFace its recommended to use naming conventions for views, API services and their shared or reusable versions.
This helps with finding views and API Services when applications have many components.

When writing DreamFace scripts, Angular directives use spinal-case (ng-app is used for the Angular directive named ngApp).
The corresponding directives which implement them use camelCase (for example ng-controller = "myController").

DreamFace component names should also use camelCase. Suggested view naming conventions are shown in the table below.
This helps to differenciate components types. The following prefixes are suggested naming conventions for DreamFace
component naming:

|

==========================   ==========  ===============
Main Components	             Prefix      Example
==========================   ==========  ===============
View (web)                   wv          wvMyView
View (mobile)                mv          mvMyMobileView
API Service Name             ALLCAPS     NEWS
API Route URL                camelCase   NEWS/getCNN
Shared View (web)            ws          wsMyWebView
Shared View (mobile)         ms          msMyMobileView
Shared DataQuery             none        No prefix
Page                         none        No prefix
Application                  none        No prefix
==========================   ==========  ===============

|
|

Shortcut Keys
^^^^^^^^^^^^^

Windows
-------

=============   ==========  ===============================
Shortcut Key	Function    Description
-------------   ----------  -------------------------------
Ctrl-S          Save        Save shortcut in View Editor
=============   ==========  ===============================


Mac
---

=============   ==========  ===============================
Shortcut Key	Function    Description
-------------   ----------  -------------------------------
⌘-S, cmd-S      Save        Save shortcut in View Editor
=============   ==========  ===============================

|
|

.. _style-gcnames-label:

Default Graphical Control Names
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Below is a list of default :term:`GC` names for all Graphical Controls in the View Editor:

|

==================   =========   ======   ===================
Graphical Controls   Group       Prefix   Default Name
==================   =========   ======   ===================
Static Text          Basic       txt      txtText1
Button               Basic       btn      btnButton1
Icon                 Basic       icn      icoIcon1
Image                Basic       img      imgImage1
HTML                 Basic       htm      htHtml1
Carrousel            Basic       crs      crsCarousel1
Treeview             Basic       trv      trvTreeView1
Input Field          Input       inp      ipnInput1
Textarea             Input       txt      txtTextArea1
Datepicker           Input       dt       dtField1
Select               Input       sel      selSelect1
Slider               Input       sld      sldSlider1
Knob                 Input       knb      knbKnob1
Chips                Input       chp      chpChips1
Rating               Input       rt       rtRating1
Richtext             Input       rch      rchText1
JSON                 Input       jsn      jsJson1
Progressbar          Input                progressBar1
Fab                  Menu        fb       fbFab1
Iconbar              Menu                 iconBar1
Treemenu             Menu        tr       trMenu1
Horizontalmenu       Menu        hrz      hrzMenu1
Radio                Selection   fld      fldRadioToggle1
Checkbox             Selection   fld      fldCheckboxToggle
Switch               Selection   swt      swtSwitch
List                 Selection   slt      sltList1
Datatable            Table       dtb      dtblDatatable1
Barchart             Chart                barChart1
Hzbarchart           Chart                hzBarChart1
Piechart             Chart                pieChart1
Donutchart           Chart                donutChart1
Linechart            Chart                lineChart1
Cmlinechart          Chart                cmLineChart1
Areachart            Chart                areaChart1
Panel                Layout      pnl      pnlPanel2
Tabs                 Layout      tb       tbTabs1
Wizard               Layout      wzd      wzdWizard1
==================   =========   ======   ===================


|

