# Secondary School Locations
# in South Dublin County council
## Data-Representation-and-Querying-Project-2015
### Author: Vusumuzi Khumalo

## Introduction
This project provides the design and documentation for the dataset Secondary School Locations which is available at  https://data.gov.ie/dataset/secondary-school-locations. The dataset is particulary taken fron the Secondary Schools in South Dublin County Council.

The data can be used mainly by teachers, lecturers and parents or guardian moving location to Dublin. 

### About the DataSet

This dataset was received in Comma Separated Values (CSV) format, and was download  from https://data.gov.ie/dataset/secondary-school-locations. The CSV file contains 18 rows, the first being a header row with the names of each field. There are twenty values which are as follows:

Field| Value
-------|-----
Department|Education
County| Name of County
School Name|Name of School
School Address|Address
Address1 |Address Line 1
Address2 | Address Line 2
Address3 |Address Line3
Address4 | Address Line4
Location| Position
Phone Number| Contact Number
Fax Number| Active Number
Email address| Contact email
Private/Public|Yes/No
Religion|Named religion
Medium of Instruction|English Only/Irish/Both
Girls/Boys Only| Yes/No
Girls| Total
Boys|Total
School Total|Boys & Girls

## Designing The API
The app should be simple enough for anybody to use but at the sametime the high standards would be upheld.

### URLs
The API is designed such that Http methods are enabled to make it user-friendly and embrace the latest technology. Some of the methods used  include: POST,DELETE, PUT and SEND.

## Total number of schools  in the South of Dublin.
You can get the total number of pupils in a particular year using the get method.
*https://data.gov.ie/dataset/secondary-school-locations/*
For example, the URL:
*http://schoolsSouthDublin.com/year/Total*
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

The POST method is one of the most important methods in webservers.Any school can  use the POST method  to send some data to the server, especially when they want to update the file.  Below is an example of  how the POST method is used to send  data to the server, which will be processed and a response will be returned:

POST http://edu.dblin.south/SecondarySchoolLocations 

####request url
A request would be sent to the Server with the data.
http://edu.dblin.south/SecondarySchoolLocations


####usage
 POST method is used to submit data which be processed to a specified resource

####response body
A response  will returned in the form of json format.
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
   
#### Put-secondary location

**PUT Method**
The PUT method is used to request the server to store the data at a location specified by the given URL. The following example requests the server to save the given  in edu.htm at the root of the server:

PUT http://edu.dblin.south/SecondarySchoolLocations

#### request url
PUT http://edu.dblin.south/SecondarySchoolLocations

#### usage
The PUT method is a useful method for requesting a server to store data.

#### response body
 ```json
   
   
   ```

#### get

#### request url

#### usage

#### response body
 ```json
   
   
   ```
   
   
#### delete

#### request url

#### usage

#### response body
 ```json
   
   
   ```














