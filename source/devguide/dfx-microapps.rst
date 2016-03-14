DreamFace MicroServices Architecture
====================================

Why DreamFace?
^^^^^^^^^^^^^^

The success of social media applications on the internet has lead to a proliferation of new and robust open source technologies.
It has also created a lot of expectations with end users for beautiful and intuitive user interfaces. At the same, IT departments
and businesses have been opening up there back-end data and applications as services through the creation of pubic and private APIs.
These new trends toward componentization and modularity have transformed application development. Developers no longer have
to create everything from scratch in monolithic projects that take too long and cost too much. Application development
today is an assembly of pieces coming from different libraries, languages, frameworks and technologies and technology continues
to evolve.

DreamFace was build in this world, to leverage these new concepts, to assemble the pieces and make developers more productive.

Businesses also want to benefit from these new development methodologies and meet their development commitments but they often don't
have a lot of experience with cloud technologies. DreamFace helps businesses to take advantage of the flexibility offered
by providing an integrated development environment with built-in and ready to use best practices for
building and deploying complex applications. It is open and extensible allowing businesses to integrate extisting code and
resources and to customize and extend their DreamFace development environment and their own applications. DreamFace was built
to help developers and businesses reap the benefits of using new components and technologies to:

* **Create modern and beautiful User Interfaces**
* **Integrete back-end data sources coming from any API**
* **Interface with existing applications and legacy technology**
* **Use containerization and virtualization to scale the applications in the cloud**

Like many frameworks and platforms, DreamFace was created to help reduce the amount of work to build consistently good applications.
There are  a lot of great developers in the world and many more will come with the new coding initiatives. The problem isn’t
really knowing how to use HTML or CSS, or Angular or any other new technology that comes along. The problem is knowing all of
the technologies necessary to build a really good application that works and scales in the cloud and that can be easily modified to
meet the ever changing business requirements.

The goal of DreamFace has always been is to compliment developer skills by providing a modular, reusable model to automate repetitive
tasks, reduce the workload of complex integration and the need to know every technology in depth. DreamFace enhances pure technology
with ready-to-use built-in best practices for error handling, API integration, security, version management, remote team development,
build management,deployment and containerization to name a few. DreamFace was created to make developers successful in delivering
consistently great applcations with a beautiful user experience.

|

Composite Apps, MicroApps and MicroServices
===========================================

DreamFace applications are a composition of reusable components.

Designing applications to run and scale in private, hybrid and public clouds can be tricky business. DreamFace was build
in the cloud and the DreamFace development environment that you use to build applications is the same application as the
runtime Web and Mobile applications build with it. All DreamFace applications are cloud-native and build with a multitenant
scalable cloud architecture. Some of the main concepts of the DreamFace architecture are:

# Applications are a collection of Microservices and MicroApps
# Applications and Data are Loosely Coupled
# Modular Application Architecture built to scale in the cloud
# Security is built-in to each layer



Applications are a collection of MicroServices and MicroApps
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

DreamFace applications are modular, built from a collection of reuable visual and data components that are combined to form
microapps or microservices, UI linked to data services that accomplish a task or an independent piece of functionality, like
a client lookup. Microservices in DreamFace are called Views and combine visual components that expose data coming from
backend services. MicroApps in DreamFace are represented as Pages which combine different Views and thier associated data
services into a composite single page application. All the components that are combined to form Views and Pages are reusable
and independent and can be combined in a different way to create any number of new Views and Pages.

DreamFace microservices and microapps are based on the concept of designing software applications as small packages of independently
deployable services. By providing self-contained, reusable components, developers can create a number of ready made microservices
and microapps that represent core application functionality. Key benefits of this modular architecture is that IT can deliver
innovative services to market more quickly, easily and affordably. Applications are also more easy to change and maintain
which gives agility for businesses to apapt to ever changing market conditions.



UI components and data services linked together acheive a function)


DreamFace applications are a composition of visual components linked Cloud applications are best deployed as a collection of cloud services, or APIs. You build up from the data to the services and then combine those services into composite services or complete composite applications.

This is service-based or service-oriented architecture, at its essence. While many understand the concepts, developers still have a tendency to create tightly coupled applications that focus on the user interface, rather than expose the underlying functions as services they can leverage independently.

When developing an application architecture for the cloud, you deal with complex distributed systems that can take advantage of loosely coupled applications built on many services that can also be decoupled from the data (see “Decouple the data” below). You can separate the application services physically, executing on the proper machine instances, and service/API managers and governance technology that provide services directories can help track the many services that make up your application.

Additional benefits may include service reuse from other applications or more coarse-grained services. You can break up applications into hundreds of underlying services that have value when used by other applications. In this way, you’re not reinventing the wheel each time you build an application. Consider the example of a credit-check service that many applications use. Combine these into a single service and the application becomes much more efficient.


Loosely Coupled
===============

Applications that are tightly coupled with the data are not well suited for the complex distributed environment of the cloud.
For an application to be able to scale, application architectures need to that separate processing and data into separate
components.

Data and processing are decoupled for the same reason that DreamFace applications are built from a collection of components
and services. When data services are decoupled, you have the option to store and process the data on any public or private
cloud instance. Data is a key asset for many enterprises and for security reasons they like to keep the data on local servers.
Most enterprises have hybrid environments where applications are deployed in the cloud. When data and applications are
decoupled they can be deployed on different hybrid environments which again brings agility to the application and allows
it to function in ever-growing distributed environment of the cloud.

DreamFace automates the connectivity to multiple data services whether the services are broadly available public services or
private APIs, DreamFace developers can leverage those services in new ways. Data sources are accessed through the servers,
enabling more security for the data and a wider range of connectivity options within applications.



Modular Composition of Reusable Components
==========================================

Extend considerations around how application components communicate to include overall performance as well. This includes
understanding how the application will scale under an increasing load.

Designing for performance means first building a model that represents how the application behaves under an increasing load.
If 1,000 or more users log on at the same time, how will the application handle the increased traffic on the network, the
increased load on the application servers, and the load placed on the back-end databases? You need to understand how
application components handle the load as the number of users increases to 1,000 or more users.

This example might increase the load on the application servers by 80 percent, the load on the network by 10 percent,
and the load on the database by 40 percent. Given that, adding 1,000 more users will likely saturate the application
servers you’ve provisioned, and you’ll need to spin up more application server instances. The network capacity might
remain the same, but the number of database instances may have to increase to handle any additional load.

Armed with this model, you can figure out how best to scale the application by automatically spinning up resource
instances that are needed. In some cases, cloud service providers offer auto-scaling capabilities, where provisioning
occurs automatically. The most efficient path, however, lies in understanding the application’s workload profile and
defining the path to scaling the application, as well as putting mechanisms in place to ensure that it will, indeed, scale.

Finally, monitor overall application performance using application-aware performance monitoring tools, and create
interfaces within the application to better enable performance monitoring. How the application provisions and de-provisions
resources should be innate to the application as well.



Application Security
====================

Often when building cloud applications, security is typically an afterthought. But for most businesses, deploying an application
in the cloud, application and data security is very important and becomes a high priotity very quickly. DreamFace cloud
application security is built into the application architecture.

Generally speaking, cloud-based applications should leverage identity and access management (IAM). Enterprises that develop
mature IAM capabilities can reduce their security costs and, more importantly, become significantly more agile at configuring
security for cloud-based applications. Indeed, IAM will be a part of more than 50 percent of existing applications that
migrate to the public cloud and nearly 90 percent of new applications built on clouds.

What’s more, the use of IAM within cloud application deployments will backfill into the enterprise, as these organizations
modernize security approaches and technologies to align with the use of public clouds. In many cases, IAM will be provided
as a service to the enterprise. This concept of cloud-delivered IAM quickly leads to the concept of centralized identity
management. As you build more cloud-based applications using IAM, each application should become significantly more secure
and more cost effective.

Your core objective is to design security into the application and take advantage of the native features of both the cloud
and the IAM system you use. However, each application has its own requirements based upon the needs of the business, and
security always differs from one enterprise to another.

Building a cloud-ready application architecture requires that you pay attention to a few new things, but many of the traditional
concepts are still important, such as sound design, testing, and learning from your mistakes. Most developers who deploy
applications on private or public cloud platforms will make some blunders, but as long as they recognize, correct, and
learn from those mistakes, they’ll be well on their way to finding a more effective path to building applications in the cloud.

Understand that approaches such as service orientation should be given priority, even if it means longer initial application
development lifecycles and bigger budgets. Even though you’ll pay more for application development in the cloud than you did for
traditional application development, the investment in services pays huge dividends year in and year out. It’s a smart investment.