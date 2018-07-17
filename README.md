<h1>Introduction to Service Design and Engineering (fall 2016) - Assignment 2</h1>

<h2>RAFFAELLA TRAN |University of Trento </h2>

<h2>Project structure </h2>

The project is divided into 6 packages:

* introsde.rest.client: contains TestClient.java, which performs requests to the server deployed on Heroku;
* introsde.rest.ehealth: contains App.java and MyApplicationConfig.java to run the standalone server;
* introsde.rest.ehealth.dao: contains LifeCoachDao.java that manages the connection to the database;
* introsde.rest.ehealth.model: contains HealthMeasureHistory.java, LifeStatus.java,MeasureDefaultRange.java MeasureDefinition.java and Person.java that represent the corresponding tables in the database. They also contain methods to query the database;
* introsde.rest.ehealth.resources: contains MeasureDefinitionResourceCollection.java, PersonCollectionResource.java and PersonResource.java. These classes declare which CRUD operations are allowed and how to perform them;
* introsde.lifecoach.wrapper - contains MeasureDefinitionWrapper.java, MeasureHistoryWrapper.java and PeopleWrapper.java used to format XML and JSON
* persistence.xml - is a file presents into folder named META-INF
* build.xml - is an ant script which automates repetitive tasks directly from the command line.
* ivy.xml - is a file which can specify the dependencies
* lifecoach.sqlite - is the database that presents an evolved data model
* client-server-xml.log - is a log file of the client calling my server using format XML format
* client-server-json.log - is a log file of the client calling my server using format JSON format

<h2> Setup </h2>

In order to clone the project and run it against the server deployed on Heroku:

git clone https://github.com/raffu12/introsde-2016-assignment-2.git
Run client with Heroku

My HEROKU server link: https://introsde-2016-assignment2.herokuapp.com/sdelab

For using it, execute:

cd introsde-2016-assignment-2
ant execute.client
After running the client, you will see two new files:

client-MyServer-json.log
client-MyServer-xml.log
