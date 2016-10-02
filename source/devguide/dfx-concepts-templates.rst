.. _dfx-templates-label:

Templates
=========

Templates are a powerful concept in DreamFace providing a way to accelerate the creation of an application. Templating allows
developers to save DreamFace components as models and lock their functionality. Those models can then be reused and only
properties that are not locked can be modified. This means by adoption of some templating functionalities.


Description
^^^^^^^^^^^
TEMPLATES are provided for all all visual application components in DreamFace: Pages, Views and Graphical Controls.

A TEMPLATE is an instance of another Object, where its properties have been set to specific values. Every property in
the base object can be locked from future changes. We cannot extend (i.e. add) properties to the base level objects.

**Example**

Create a BUTTON, choose class = md-no-ink md-primary, lock ALL attributes except Label/Icon/onClick. Save
this TEMPLATE as “Button model1”. In this scenario, a developer can get this Button model from the pre-defined graphical
controls list and use it in an application. Only the three specified properties Label/Icon/onClick can be modified.

Every graphical control has an attribute (like its ID) that refers to the *Template* it uses. Templates are by definition,
recursive, and developers will need to navigate the TEMPLATE LIST until to get to the base object.

A Visual way to show TEMPLATES should be provided from the GC list
Show them grouped by category
Under Button, see categories such as CONFIRM (under which we have few buttons with the Accept label, icons, different
sizes, etc.) or ALERT (same description)...
Be able to put a description on each of the TEMPLATE objects
Be able to filter and search this list
Later, show a hierarchy of these objects
Maybe show their HTML?

TEMPLATED objects show like on a screen (i.e. rendered) for clarity of choice and can be dragged and dropped directly from there
A TEMPLATE can be elected to become the DEFAULT; This should allow that TEMPLATE to become the default one used when someone drags the category (aka BUTTON). By default, the product ships with a default button that is using a file that has all the classes needed for the default GC
An update of the TEMPLATE should be possible; Show the rendering of the new one; show new and old at the same time
TEMPLATES are part of the Application assets (or settings?) that can be copied between an app and another (or over to Github…)
Even complex objects such as DataTable or Panel should be templatable. Basically, we take the DEFAULT JSON, we add attributes (so the JSON is modified) and “lock” the changes on some of these attribs and give a subset of properties for users to edit

|

Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.
