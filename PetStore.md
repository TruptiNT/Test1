

# Fetch a List of Pets

This section describes the procedure to fetch a list of pets from the [Swagger Pet store API](https://petstore.swagger.io/) through API interaction.


### Endpoint
       GET /pet/findByStatus

### Description
Finds pets by status.
Multiple status values can be provided with comma separated strings.

       
### Parameters

| Name|Description|Type  |Default|
|--------|-------------------------------------------------------------------------------------------|------|------------|
| status |Status values that need to be considered for filter (values are: available, pending, sold). The field is mandatory |query | available
| N/A|Nones mandatory |header| available
| status |Status values that need to be considered for filter (values are: available, pending, sold). The field is mandatory |query | available
| status |Status values that need to be considered for filter (values are: available, pending, sold). The field is mandatory |query | available


### Request

#### Request in cURL
//Request URL to find pets with the status **available**: 

    https://petstore.swagger.io/v2/pet/findByStatus?status=available

#### Request in Java 
// This code sample uses the 'Unirest' library: 
// http://unirest.io/java.html 

    HttpResponse<String> response = Unirest.get("https://petstore.swagger.io/v2/pet/findByStatus") .header("Accept", "application/xml") .queryString("status", "{status}") .asString(); System.out.println(response.getBody());


### Response

#### Response Content Type
-   application/xml
-   application/json

#### Response Code

| HTTP Code       |Description                          |           
|--------------|-------------------------------|
|200           |Successful operation   
|400           |Invalid Status code

### Examples

#### cURL

//Request URL to find pets with the status **available**: 

    https://petstore.swagger.io/v2/pet/findByStatus?status=available
    
The following is an example of a successful  response with status **available**:

    {
    "id": 1234,
    "category": {
    "id": 0,
    "name": "Dog"
     },
    "name": "Zero",
    "photoUrls": [
     "string"
     ],
     "tags": [
     {
     "id": 0,
     "name": "string"
     }
    ],
     }

#### Postman
In Postman, enter the URL:  

     http://petstore.swagger.io/v2/pet/findByStatus?status=available 

  The following is an example of a successful  response with status **available**:
  

    `[ 
      { 
      "id": 2154, 
      "category": 
       { 
        "id": 2154, 
        "name": "<string>" 
       }, 
     "name": "doggie", 
     "photoUrls": [ "<string>" ], 
     "tags": 
     [ 
     { 
     "id": 2154, 
     "name": "<string>" } 
    ], 
    "status": "available" }
     ]`



<!--stackedit_data:
eyJwcm9wZXJ0aWVzIjoidGl0bGU6IFBldFN0b3JlXG5hdXRob3
I6IFRydXB0aVxuc3RhdHVzOiBGcnN0IGRyYWZ0XG5kYXRlOiAy
Mi0wMy0yMDI0XG4iLCJoaXN0b3J5IjpbLTE0MzU5MzQzNjAsLT
E5MjQ1ODc1NDUsODE2NTAyNDA2XX0=
-->