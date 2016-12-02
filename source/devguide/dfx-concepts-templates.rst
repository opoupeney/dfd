.. _dfx-templates-label:

Templates
=========

Templates are a powerful concept in DreamFace providing a way to accelerate the creation of an application. Templating allows
developers to save DreamFace components as models and lock in their functionality. Those models can then be reused and only
properties that are not locked can be modified. This means by adoption of some templating functionalities.


Description
^^^^^^^^^^^
*Templates* can be provided for all visual application components in DreamFace: Pages, Views and all Graphical Controls.

A Template is an instance of a component, where its properties have been set to specific values and saved. Every property in
the base object or component can be locked from future changes. In this way, templates could be prepared for different
components and used by developers when creating an application. This guarantees a consistent look and feel and behavoir
across the application. Developers would start developing a component from a template and modify only the properties that
are unlocked. New properties cannot not be added (i.e. add) to the base level component.

**An Example of a template**

Create a BUTTON, choose class and set to *md-no-ink md-warn*, lock ALL attributes except Label/Icon/onClick. Save
this :term:`template` as “Button model1”. In this scenario, a developer can get this Button model from the pre-defined graphical
controls list and use it in an application. Only the three specified properties Label/Icon/onClick can be modified.

Each graphical control has an :term:`template` property which is set to set to *default*.

|

Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.
