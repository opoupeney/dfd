
.. _style-label:

Programming Style Guide and Naming Conventions
==============================================


Conventions in the Widget Editor
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

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


Naming Conventions
^^^^^^^^^^^^^^^^^


DreamFace component names may only contain alphanumeric characters. Numbers are permitted and are generally used when creating many of the same type of control.
Do not use underscores, hyphens, or any other non-alphanumeric character. Spaces are not allowed, they will be accepted without errors in some circumstances but will
ultimately cause problems.

Within DreamFace its recommended to use naming conventions for widgets, queries, their shared or reusable versions.
This helps with finding widgets when applications have many components.

When writing DreamFace scripts, Angular directives use spinal-case (ng-app is used for the Angular directive named ngApp). The corresponding directives which implement them use camelCase (for example ng-controller = "myController").

DreamFace component names should also use camelCase. Suggested widget naming conventions are shown in the table below. This helps to differenciate components types.
The following prefixes are suggested naming conventions for DreamFace component naming:

|

==========================   ======   ===================
Main Components	             Prefix   Example
==========================   ======   ===================
View (desktop)	             view     *viewMyView*
View (mobile)                mview    *mviewMyMobileView*
API Route	                 r        *rMyRoute*
Shared DataView (web)	     ws       *wsMyWebView*
Shared DataView (mobile)     ms       *msMyMobileView*
Shared DataQuery 	         qs       *qsMyDataQuery*
Screen                       none     No prefix
Application                  none     No prefix
==========================   ======   ===================

|

Suggested naming conventions for graphical controls:

|

==================   ======   ===================
Graphical Controls   Prefix   Example
==================   ======   ===================
Static Text          txt      txtText1
Link                 lnk      lnkLink1
Button               btn      btnButton1
Image                img      imgImage1
Input Field          fld      fldInput1
Textarea             fld      fieldTextArea1
Checkbox             fld      fldCheckbox1
Combobox             fld      fldCombobox1
Radio                fld      fldRadio1
DataGrid             grid     gridDataGrid1
Chart                ch       chChart1
HTML                 fld      fldHTML
Rating               rt       rtRating1
Slider               sl       slSlider1
Knob                 kn       knKnob1
Radiotoggle          fld      fldRadioToggle1
Checkboxtoggle       fld      fldCheckboxToggle
Carousel             cr       crCarousel1
Panel                pnl      pnlPanel
Tabs                 pnl      pnlTabs1
Accordion            pnl      pnlAccordion1
Wizard               wzd      wzdWizard1
==================   ======   ===================

|
|
