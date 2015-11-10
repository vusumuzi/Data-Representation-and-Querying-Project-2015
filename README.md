# Secondary School Locations
## Data-Representation-and-Querying-Project-2015
### Vusumuzi Khumalo

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
The API is designed such that Http methods are enabled to make it user-friendly and embrace the latest techology. Some of the methods that are include: the POST, PUT and SEND.

## Total number of schools  in the South of Dublin.
You can get the total number of pupils in a particular year using the get method.
*https://data.gov.ie/dataset/secondary-school-locations/*
For example, the URL:
*http://schoolsSouthDublin.com/year/Total*
will return a list of schools and the total numbers of pupils.
The data will be returned in JSON format, with the following properties:
    - *year*: the year in question.
    - *total*: the total enrollment for the year.
    ...
An example of a response would be:
    ```json
    [ {"year": 2012, "total": " 5000", ...}, {...}, ...]













