Creating API Services
=====================

API Services are a kind of the data access component of DreamFace.

constructed queries which allow extracting data from external or inner sources and represent
them in a structured view.

Adding, finding, and editing DQ (DataQueries) are performed in Dashboard.

.. image:: images/creating-queries/dfx-dq-01.png


Adding DQ is performed with a button “**+ Query**”, and finding is performed with a magnifying glass icon. If you press this icon without typing any characters, all DQ will be listed.

Found DQ are listed at the right side of the screen:

.. image:: images/creating-queries/dfx-dq-02.png
	:width: 500px

Creating a new DataQuery consists of several important fields.

.. image:: images/creating-queries/dfx-dq-03.png
	:width: 500px


Use the following parameters to set up a new DataQuery.


**Query Parameters**



=====================================  =========================================================================
Parameter                              Possible Values and Description
=====================================  =========================================================================
**Properties**                         —
Name                                   String without spaces
Description                            Human description
Format                                 JSON / XML
Persistence                            None / Sessions to save activity of the query
Category                               Add and select categories to organize your Queries

**Query Connector Settings**           —
External Source / DataBase             Choose one to specify a data source
Request URL                            URL specified with the REST API of a Provider
Request Type                           POST / GET / PUT depending of your actions
Provider                               Selected value from the list of AuthProviders
                                       specified in the Settings of DFX
Request Body                           Used if the Request Type is “POST” to send data in JSON or XML format

**Query Parameters**                   —
Name                                   Key name of a parameter (i.e. “screen_name”)
Action                                 “equal” as a single value
Value                                  Value of the parameter transferred
Type                                   request / header / url

**Application Exceptions**             —
Name                                   Name of error
RegExp                                 Regular expression which is a mask of an exception

**Pre DataQuery execution**            —
Name                                   Arbitrary name of a code fragment
Code Execution                         Link to edit the code
Order                                  Interface elements allowing move codes and set their order of execution

**Post DataQuery execution**           —
Name                                   Arbitrary name of a code fragment
Code Execution                         Link to edit the code
Order                                  Interface elements allowing move codes and set their order of execution
=====================================  =========================================================================



Pay attention to the following fields, which are determinative for creating a new DQ and getting a correct result:

* **Name**, to invoke a DQ directly
* **Format**, to specify how the data are structured
* **All fields** related to Query Connector to get data

It is important to choose one of methods (called **Request Type** here); now "GET", "POST" and "PUT" methods are entirely supported.

When adding *Query Parameters*, it is important to make differences between the following *Query Types*: "request", "header", and "url" type.

"Request" is similar to "Query String" with a string of key and values set as GET request; "url" type allows to create clean URL parsed as a query string. E.g., if Query Type is "url", one can create URLs like ``http://website.com/John/video``, where ``John`` and ``video`` are parts responding to the mask ``http://website.com/{profile}/{content}``.


The main part of DQ parameters is concentrated in the 2nd part: *Query Connector Settings*. By default, data are transferred with “GET” method (“Request Type”). But if you choose “POST” request type, you get the possibility to pass more complex sets of data, i.e. JSON formatted, while a new field “Request Body” is opened:

.. image:: images/creating-queries/dfx-dq-04.png
	:width: 500px


One should choose one of the 3 types of sources: External Source, or DreamFace DataBase, or External DataBase.


**1. External Source**

In this case you should specify Authorization Provider, if the performing of requests implies authorization. I.e. the 1st step to do is to create a Provider, and it will be listed in the drop-down list of Providers.

For example, if you have to work with Twitter API, you have to sign in at https://dev.twitter.com/ with your Twitter credentials and use it to create an application corresponding to the DFX tasks. Open the dropdown menu under your profile image and click on “My applications”. Click the large button “Create New App” and fill all fields. Then confirm the Developer Rules and save the new application. Return to the application list, choose the created one and set its Permissions to “Read and Write”. Update settings and open “API Keys” tab. Regenerate keys. Finally, open DFX administrative interface, open Settings at the top menu and create a new item in “AuthProviders” section; specify auth protocol as OAuth1 and use the secure data from the created Twitter application.

.. image:: images/creating-queries/dfx-tw-004-addprovider.png
	:width: 500px


Now using Twitter API, you can perform requests, e.g.: ::

	[Request URL] = https://api.twitter.com/1.1/statuses/user_timeline.json
	[Request Type] = GET

Here you should add 2 parameters at the section below: ::

	[screen_name] = your_screen_name
	[count] = 10

This example allows getting 10 recently published Twitter posts from your timeline.


Or, if one needs to post entries in Twitter: ::

	[Request URL] = https://api.twitter.com/1.1/statuses/update.json
	[Request Type] = POST
	[Request Body] = {"status": "your new twitt text"}


**2. DreamFace DataBase**

Provider field is disabled in this case.

This choose is suitable when you use internal database for storing various user data. The default value for “Request URL” parameter is http://localhost:3000/database — if you keep and run the database at the local storage. But you can specify a collection to use in order to minify the diapason of data selected. To perform it, click on the icon at the right side of “Request URL” field, and then select a necessary database or collection; the correct path will be placed at the “Request URL” field:

.. image:: images/creating-queries/dfx-dq-05.png
	:width: 500px


Specify a collection, execute a query, and at the tree of the reached result you can see the “data” node, which contains the set of data from the database.


**3. External DataBase**

Provider field is disabled in this case. But one have to set up a new database connection before working with this possibilities.

Open “Settings” at the top menu and create a new database provider.

.. image:: images/creating-queries/dfx-dq-06.png
	:width: 500px


You can specify any existing database for the direct access. Now DFX supports MySQL and MSSQL database drivers.

Now, when you go back to the creating of a new DQ with an access to an external database, you can specify the created database driver; in the case if you specified a database, you get direct access to its tables:

.. image:: images/creating-queries/dfx-dq-07.png
	:width: 500px

Select a table, make sure that the “Request URL” field has been changed, and execute the DQ with pressing the button “Execute” at the right side of the screen. Make sure that the data is received.

.. image:: images/creating-queries/dfx-dq-08.png
	:width: 300px


There is a new useful feature for developers: View Request. At the latest versions of DFX, you can see the request which has been executed. Use the link "View Request" at the DataQuery definition screen.

.. image:: images/creating-queries/dfx-dq-08-x.png
	:width: 300px

There are two types of **filters** which can follow the main DataQuery: so-called Pre Codes and Post Codes (or Pre DataQuery Execution, and Post DataQuery Execution).

This means that you can run additional JavaScript code before and after launching Queries. If you specify Pre Codes or / and Post Codes, they will be executed too. “Pre DataQuery execution” allows to specify one or a set of code fragments which will be executed before the current Query, and the “Post DataQuery execution” allows to specify one or a set of code fragments which will be executed after it runs.

In order to test them, click to add Pre Code, add name and edit the script which will be executed. Then save and exit to return to the editing the Query.


**Pre Code examples**

Using params variable as an array: ::

	if(params[0].name == 'lng' && params[0].value == 'en') params[0].value = 'EN';
	if(params[0].value =='en'){ abortQueryExecution({"name":"abort Execution"}); }

Also, one can change parameters in the Pre Code: ::

	executeQuery({"qName":"qExtServer"}, function(res){
	   params.push( {
	   'name':'params',
	   'value':encodeURIComponent(JSON.stringify(res)),
	   'type':'request'
	   });
	   terminateFilter();
	});


**PostCode examples**

System ``response`` variable can be used as JSON formatted set of data.


First example: ::

	var countries = response.countries;
	countries.push({'country':'Ukraine', 'capital':'Kiev'});

ExecuteQuery as a Post Code:

1) without parameters (the callback function used here is launched when the query has been executed; terminateFilter() allows stopping the following execution of the functions) ::

	executeQuery({"qName":"qTwitterGet"}, function(res){
		response.my_twitter = res;
		terminateFilter();
	});

2) with parameters ::

	executeQuery({"qName":"qMikhail","params":{"count":3}}, function(res){
		response.mikhail_twitter = res;
		terminateFilter();
	});


The resulting data can be received too much.

In this case there can be helpful two functions: ``filterProperties()`` and ``filterData()`` to decrease the amount of received data in order to deal with necessary ones only.


Example for ``filterProperties()``: leave only those properties that we need ::

	filterProperties(response, ['created_at','text'], function(res){
		response = res;
		terminateFilter();
	});

As the result of the execution of this code the set of values in response variable is reduced to the specified ones.

Example for ``filterData()``: leaving data that satisfy our condition. Here we can use operators: ``eq`` (equal), ``ne`` (not equal), ``lt`` (less then), ``gt`` (greater then) ::

	filterData(response, 'name', 'eq', 'Helen', function(res){
	   response = res;
	   terminateFilter();
	});

The data received are filtered that we have only results where the value of “name” field is equal to “Helen”.


The set of these functions:

* executeQuery()
* filterProperties()
* filterData()

is called “Orchestration of Queries”; it helps making queries more flexible and avoid getting unnecessary data.