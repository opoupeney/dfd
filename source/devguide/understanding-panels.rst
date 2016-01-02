.. _panels-label:

Understanding Layouts and Panels
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

DreamFace uses :term:`Angular Material` for most of the pre-defined graphical control provided in the View Editor and for
the underlying design of the DreamFace Studio. Angular Material is a UI component library based on Google
:term:`Material Design`. It is similar to :term:`Bootstrap` since it provides UI components, a grid system and angular
directives for their use. The Angualr Material layout is based on is based on the Flexible Box Layout specification, which
is a W3C standard Flexible Box. As the name implies this layout system gives more flexibility to the layout. DreamFace panels
use the Angular Material layout system to organize graphical controls within a View.


DreamFace Panels
----------------
DreamFace panels uses a grid system of rows and columns to create view and screen layouts.
Similar to the Bootstrap grid system, DreamFace uses panels containing layouts of multiple rows and columns.
Each row can be divided into one or more columns, with a maximum of twelve columns possible.
Columns can be grouped together in spans. A span groups together one or more columns to create fewer but wider columns as seen in the table below.
In DreamFace, it's recommended that you create rows with 3 or 4 columns maximum to maintain readability.
Whatever number of columns you choose to span, the total should add up to twelve.
For example, if you could create a row with 2 columns, each with column spans of 6, that would add up to twelve.
DreamFace does not check if the number of columns and column spans adds up to twelve, it will however, affect the size and alignment of your screen.

Below are some examples of how a row can span columns to create fewer and wider columns.

.. image:: ../images/devguide/dfx-grid-system.png


The DreamFace grid system is responsive, and the columns will re-arrange automatically based on the screen size.
On a big screen it might look better with the content organized in three columns, but on a mobile screen it will be more readable if the content items (columns) are stacked on top of each other.


Creating Layouts in the view Editor
-------------------------------------

DreamFace uses a grid system with panels of multiple rows and columns to determine the layout of graphical controls displayed a view.

When you arrive in the view Editor to create a new view, at the top of the canvas DreamFace creates a default panel with a layout of one row and one column with a span of twelve.
In fact, each time you create a new panel, by default, DreamFace creates the panel with one row and one column with a span of twelve.

The default panel has the *pnlpanel1*. Successive panels that are created get the same name with the number corresponding to their order of creation, so the fourth panel created would have the name *pnlpanel4*
The default panel has a :term:`controller` which contains all of the script for the view. Each panel can have a controller associated with it but all scripting for the view is contained in the default panel controller.

.. image:: ../images/devguide/dfx-grid-1row.png

Panels have the following a hierarchy of organization: Panel -> Layout -> Row -> Column.

If you click on the outer border, or the word Panel in the properties window, the panel properties will be displayed in the view Properties window on the right.

If you click on the word Layout it will show that the panel has one row with one column with a span of twelve. You can add a row, then click on layout again to show that another row with one column, span of twelve was created.

To begin creating your view you drag pre-built graphical controls into a column. You can create the panel layout from the beginning if you know it the layout that you want or you can add rows and columns to organize your panel layout as you need them.

**DreamFace grid system rules for views:**

* Rows are part of a panel layout
* Rows are divided into horizontal groups of columns
* Columns can span one or more columns, grouping them together to form a larger, wider column.
* The number of columns spanned in a row should add up to twelve columns maximum.
* Grid columns are created by specifying the number of columns you wish to span. For example, three equal columns would have a width or span of 4 columns each.
* Graphical Controls are placed in columns, and only graphical controls can be the immediate children of columns and only columns can be immediate children of rows.
* Rows are created successively from the top to the bottom of the the view layout. It is not possible to insert a new row within existing rows or move a row. You will need to add a new row at the bottom and move graphical controls into that row.
* There is no limit to the number of rows you can add to a panel in a view.

Using the Grid System for Field Alignment in Dataviews
--------------------------------------------------------

The grid system can be used to align and organize graphical controls.
Orientation, alignment and disposition are defined at the column level.
Select a column and the main column properties appear in the properties window on the right.
|

.. image:: ../images/devguide/dfx-col-properties.png

|

The table below containing possible values for each.

Orientation refers to vertical or horizontal alignment in a column.
Alignment refers to the alignment of pre-build graphical. Alignment can be at the *start* of the column, centered, at the right of the row.
Disposition refers to the orgainzation within the column, start, center and end are intuitive, *space around* means take all components within a row

|

===========  =========================================================
Type         Possible Values
===========  =========================================================
Orientation  *horizontal*, *vertical*
Alignment    *start*, *center*, *end*, *vertical*, *horizontal*
Disposition  *start*, *center*, *end*, *space around*, *space between*
===========  =========================================================

If you choose to align horizontally, for example 3 graphical control buttons and you want to add an input field above, you will need to create another row.



Creating Layouts in Screens
---------------------------

DreamFace screens use the same grid system of rows and columns to create screen layout as with the views. The screen layout uses the same grid system of rows and columns as the views, each row having up to twelve columns maximum.
When you create a screen in DreamFace it has no rows. Each new row that is added will start with one column with a span of twelve. You can modify the number of columns to create more than one column. Each column can span a number of smaller columns,
for example a row with two equal sized columns would have each column spanning 6 smaller columns, with the maximum number of columns being twelve. For readability it is recommended to create fewer, larger columns, we recommend a maximum of four columns for readability.
The composition of rows and columns on the screen will be the screen layout. Dataviews are placed inside the screen columns you.

|

.. image:: ../images/devguide/dfx-screenlayout.png


**DreamFace grid system rules for screens:**

* When a screen is created it has no rows or columns.
* A screen needs to have a minimum of one row and one column to display Dataviews.
* Rows are divided into horizontal groups of columns.
* Dataviews (containing their own layout) are placed in columns,
* Only Dataviews can be the immediate children of columns and only columns may be immediate children of rows in a screen.
* Grid columns are created by specifying the number of 12 columns you wish to span. For example, three equal columns would have a width or span  of four columns each.
* There is no limit to the number of rows you can add to a screen.

|
|
