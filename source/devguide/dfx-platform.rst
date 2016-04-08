Understanding the DreamFace Platform
====================================


DreamFace is a :term:`native cloud application`. The applications that you build with DreamFace are also :term:`cloud-native`
applications. Support for :term:`multitenancy`, :term:`containerization`, :term:`virtualization` and other fundamental
cloud technologies is at the core of the product.

When installed for the first time, a DreamFace :term:`platform` is available to create tenants (see :term:`multitenant` for
the various purposes of application development:

.. image:: ../images/diagrams/dfx-cloud-platform.png
   :width: 700px

* One DreamFace platform can create one or more tenants (such as Development, UAT or Production as seen in the diagram above)
* One Tenant can be used to create one or more applications (Web or mobile)

In **BlueMix**, you arrive directly in your cloud tenant and start developing there rightaway. A BlueMix tenant has an id
and can be used to create one or more applications.

It is important to note that the creation of tenants under the same platform is an instantaneous action, using the same
code base of the underlying installed DreamFace platform. Under the hood, DreamFace creates a JSON object that maps to
the tenant in the Global JSON DataStore. The DreamFace Platform has some global attributes that can be used for all tenants
under the Platform, such as the developers and their roles or the deployment features supported by the Platform (Docker
interface for dockerization of your application, deployment on Bluemix, etc.).

|

Platform vs. Framework
----------------------

You may be wondering why we call DreamFace a platform. In this section we'll break it down and explain why it's more than
a framework.


DreamFace is a Platform-as-a-Service (PaaS) which helps developers create and deploy Software-as-a-Service (SaaS) applications.
That already qualifies DreamFace as a platform. In addition, DreamFace goes beyond a framework (code libraries, scripting
language, APIs, ...) proposing several enterprise features:


* Build-in Editors

  * a visual (drag-n-drop) View Editor
  * a Scripting Editor for writing code with code assistants (scripting is in standard javascript / angular)
  * a Page Editor
  * a Page Template Editor
  * an API Service Object / Services / Routes editor with with introspection of meta-data and pre / post treatment of APIs

* a local database
* a JSON repository containing the definition of all application components (allows for injecting from external sources like BPM)
* Github integration for team development
* Slack integration for team collaboration
* a compiler and build manager
* automatic deployment to the cloud
* built-in on touch dockerization

and many other enterprise bells and whistles.

DreamFace goes far beyond scripting and libraries to provide a complete enterprise platform. As DreamFace is a :term:`Node`
module, DreamFace can be used to enhance other Node modules and platforms.

|


Return to the `Documentation Home <http://localhost:63342/dfd/build/index.html>`_.




