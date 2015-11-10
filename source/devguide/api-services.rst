.. _apiservices-label:

API Services
============

An API Service is a DreamFace component that is used to consume public, private or internal APIs. API Services are defined by Properties and API Routes.

An API Service is composed of one or more API Routes and is a logical grouping of API Routes under a single entity, that maps that route or service with a client side service.

We can differentiate API Services into several categories depending on their authentication requirements :

* **Simple API Services** are API Services which do not require authentication, for example an RSS feed or a url like the github api api.github.com/users Simple API Services have the following characteristics, they :

    * Can be called from the browser and therefore from javascript in the browser
    * Return data in JSON format which can be converted into javascript ojbects and easily consumed
    * Do not require authentication or any client key

* **API Services with Basic Authentication** these API require Basic Authentication which is used to create a key based on username and password of the user account
* **API Services with oAuth2 Authentication** these are API Services that are related to personal data and require more extensive Authentication and Acknowlegement and Authorization to use tha personal data

    * Key to consume the API (Google Translate, Goooge) authenticates the application to consume the API token and secret
    * Personal data - the user needs extension to oAuth1 application neeeds to be authenticated and user needs to accept or decline that the applicatio

|

Properties
^^^^^^^^^^

Properties of the API Service include :

* **API Service Name** - the name of the API service on the server
* **Description** - a description of what the API Service does
* **Category** - The Category that the API Service being defined belonds too. This is a logical grouping of API Services, for example News would contain services accessing news.
* **Angular Service Name** - This is the name of the Angular Service on the client side.

|

API Routes
^^^^^^^^^^

API Routes can be defined and tested without any codeing, just set the parameters that define the desired connector and test it. The API Routes are listed in the
API Routes section. By clicking on a given API Route, you can change Settings & Parameters for an API Route. You can set Filters and test the functioning of the
API Route under Simulate.

|

Settings & Parameters
^^^^^^^^^^^^^^^^^^^^

Settings & Parameters for API Routes contain

* **Main Properties** The Main Properties contain API Route URL which is a name given to the route. This can be modified and can contain any name.
* **Connector Settings** The Connector setting define several parameters:
    * Conncector Type
    * Request URL
    * Request Type (REST, ...)
    * Data Format Received
    * Authentication Provider
    * Angular Service Function
* **Parameters** - used to define parameters to send to the service in the service call.

|

Filters
^^^^^^^


|

Simulate
^^^^^^^^

Once the Setting & Parameters are defined, you can go to the Simulate tab and test to see if your your API Route is functioning properly. Among the tests
you can perform :

* View Meta Data - will return all of the Metadata from the service call
* View Result - will return the results (data) from the service call
* View Request - will display the request that was sent off to the service. This is used mainly to view the Request that was sent to the service for debugging purposes.

