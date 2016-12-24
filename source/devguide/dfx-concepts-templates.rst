.. _dfx-templates-label:

Templates
=========

Templates are a powerful concept in DreamFace providing a way to accelerate the creation of an application. Templating allows
developers to save DreamFace components as models and lock in their functionality. Those models can then be reused and only
properties that are not locked can be modified thus standarizing some properties across an application.


Description
^^^^^^^^^^^
*Templates* can be provided for all visual application components in DreamFace: Pages, Views and all Graphical Controls.

A Template is an instance of a component, where its properties have been set to specific values and saved. Every property in
the base object or component can be locked from future changes. In this way, templates could be prepared for different
components and used by developers when creating an application. This guarantees a consistent look and feel and behavoir
across the application. Developers would start developing a component from a template and modify only the properties that
are unlocked.

**An Example of a template**

Create a BUTTON, choose class and set to *md-no-ink md-warn*, lock ALL attributes except Label/Icon/onClick. Save
this :term:`template` as “button_model1”. In this scenario, a developer can get this Button model from the pre-defined graphical
controls list and use it in an application. Only the three specified properties Label/Icon/onClick can be modified by the
developer.

Each graphical control has a :term:`template` property which is set to set to *default*.

Templates are not available for use at this time. They are a part of the roadmap and will be added soon.

Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.
