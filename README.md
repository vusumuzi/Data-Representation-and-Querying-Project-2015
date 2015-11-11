# Secondary School Locations in South Dublin County council
## Data-Representation-and-Querying-Project-2015
### Author: Vusumuzi Khumalo

## Introduction
This project provides the design and documentation for the dataset Secondary School Locations which is available at  https://data.gov.ie/dataset/secondary-school-locations. The dataset is particulary taken fron the Secondary Schools in South Dublin County Council.

The data can be used mainly by teachers, lecturers and parents or guardians moving location to Dublin and  any individuals who are interested looking for particular schools that is whether the school is in the city or in the periphery.

### About the DataSet

This dataset was received in Comma Separated Values (CSV) format, and was download  from https://data.gov.ie/dataset/secondary-school-locations. The CSV file contains 18 rows, the first being a header row with the names of each field. There are twenty values which are as follows:

Field         | Value
--------------|--------
Department    |  Education
County        |  Name of County
School Name   |  Name of School
SchoolAddress |  Address
Address1      |  Address Line 1
Address2      |  Address Line 2
Address3      |  Address Line3
Address4      |  Address Line4
Location      |  Position
Phone Number  |  Contact Number
Fax Number    | Active Number
Email address | Contact email
Private/Public| Yes/No
Religion      | Named religion
Language Used |English Only/Irish/Both
Girls/BoysOnly| Yes/No
Girls         | Total
Boys          |Total
School Total  |Boys & Girls

### Designing The API
The app should be simple enough for anybody to use but at the sametime the high standards would be upheld.

### URLs
The API is designed such that Http methods are enabled to make it user-friendly and embrace the latest technology. Some of the methods used  include: POST,DELETE, PUT and SEND. 

###Http Methods

Method     |  Description
-----------|---------------
**GET**    |  Requests data from a specified resource
**POST**   |  Submits data to be processed to a specified resource
**HEAD**   |	Same as GET but returns only HTTP headers and no document body
**PUT**    |	Uploads a representation of the specified URI
**DELETE** |	Deletes the specified resource
**OPTIONS**|	Returns the HTTP methods that the server supports
**CONNECT**|	Converts the request connection to a transparent TCP/IP tunnel

## Total number of schools  in the South of Dublin.
You can get the total number of pupils in a particular year using the get method.
*https://data.gov.ie/dataset/secondary-school-locations/*
For example, the URL:
*http://schoolsSouthDublin.com/year/total*
will return a list of schools and the total numbers of pupils.
The data will be returned in JSON format, with the following properties:
    - *year*: the year in question.
    - *total*: the total enrolment for the year.
    ...
An example of a response would be:
    ```json
    [ {"year": 2012, "total": " 5000", ...}, {...}, ...]
    ```

####Post-add secondary location

http://edu.dblin.south/SecondarySchoolLocations

**POST Method**

The POST method is one of the most important methods in Https. Any school can  use the POST method  to send some data to the server, especially when they want to update the file.  Below is an example of  how the POST method is used to send  data to the server, which will be processed and a response will be returned:

POST http://edu.dblin.south/SecondarySchoolLocations 

####request url
A request would be sent to the Server with the data.
http://edu.dblin.south/SecondarySchoolLocations


####usage
 POST method is used to submit data which be processed to a specified resource

####response body
A response  willbe returned in the form of a json format.
   ```json
   "Organisation":"DEPARTMENT OF EDUCATION AND SCIENCE",
    "Name":"SCOIL NAOMH MAELRUANS",
    "Address1":"OLD BAWN AVENUE",
    "Address2":"TALLAGHT",
    "Address3":"DUBLIN 24",
    "Address4":null,
    "ITMEast":"709200.334",
    "ITMNorth":"726528.533"
   ```
   
#### Put-secondary locations

**PUT Method**

The PUT method is used to request the server to store the data at a location specified by the given URL. The following example requests the server to save the given  in edu.htm at the root of the server:

PUT http://edu.dblin.south/SecondarySchoolLocations

#### request url
PUT http://edu.dblin.south/SecondarySchoolLocations

#### usage
The PUT method is a useful method for requesting a server to store data.

#### response body
 ```json
   "Organisation":"DEPARTMENT OF EDUCATION AND SCIENCE",
    "Name":"SCOIL NAOMH MAELRUANS",
    "Address1":"OLD BAWN AVENUE",
    "Address2":"TALLAGHT",
    "Address3":"DUBLIN 24",
    "Address4":null,
    "ITMEast":"709200.334",
    "ITMNorth":"726528.533"
   ```
### get-secondary locations

**GET Method**

A GET  method is the main method which is used for retriving documents. The  GET request method retrieves data from a web server by specifying parameters in the URL portion of the request. . The following example illustrates how the  GET method is used to retrieve edu.secondaryschools.htm:
GET /edu.secondaryschools.htm.

#### request url
GET http://edu.secondaryschools.htm.

#### usage
To get particular information about schools in South Dublin County Council one would use the GET method which retrives the data from the server and send it back to the user. For instance if one is looking for schools which is boys only the URL would be http://edu.dblin.south/SecondarySchoolLocations/boys

#### response body
 ```json
   "Organisation":"DEPARTMENT OF EDUCATION AND SCIENCE",
    "Name":"SCOIL NAOMH MAELRUANS",
    "Address1":"OLD BAWN AVENUE",
    "Address2":"TALLAGHT",
    "Address3":"DUBLIN 24",
    "Address4":null,
    "ITMEast":"709200.334",
    "ITMNorth":"726528.533"
   ```
#### delete-secondary locations

**DELETE Method**

Files may hold information which is outdated or irrelevant. The DELETE method is therefore used to request the server to delete a file at a location specified by the given URL. The  example at the bottom shows how a  request is sent to the server to delete the given file at the root of the server:

DELETE /http://edu.dblin.south/SecondarySchoolLocations/boys

#### request url
http://edu.dblin.south/SecondarySchoolLocations/boys

#### usage
If the school needs to get rid of absolete data, a delete method would be appropiate to use. For example if a particular school wants to delete all the files that were created in 2002, the URL would look like like this:
DELETE http://edu.dblin.south/SecondarySchoolLocations/girls/2002

#### response body
 ```json
   json
   "Organisation":"DEPARTMENT OF EDUCATION AND SCIENCE",
    "Name":"SCOIL NAOMH MAELRUANS",
    "Address1":"OLD BAWN AVENUE",
    "Address2":"TALLAGHT",
    "Address3":"DUBLIN 24",
    "Address4":null,
    "ITMEast":"709200.334",
    "ITMNorth":"726528.533"
   
   ```
   Conclusion
   
   The API that is designed for the users has advantages and disadvantages in the sense that users do not have the capacity     to add or remove any entries.  














