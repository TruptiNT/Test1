

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
| N/A|N/A|header|  
|N/A| N/A|path| 


### Sample Request

#### Request in cURL
The sample request URL  retrieves pets with the status **available**: 

    https://petstore.swagger.io/v2/pet/findByStatus?status=available

#### Request in Java 
The sample request uses the 'Unirest' library  http://unirest.io/java.html  to retrieve pets with status **available**

    HttpResponse<String> response = Unirest.get("https://petstore.swagger.io/v2/pet/findByStatus") .header("Accept", "application/xml") .queryString("status", "{status}") .asString(); System.out.println(response.getBody());

### Response Content Type
-   application/xml
-   application/json

### Response Code

| HTTP Code       |Description                          |           
|--------------|-------------------------------|
|200           |Successful operation   
|400           |Invalid Status code

### Sample Response

#### cURL

The following is an example of a successful response with 2 records with status **available**:

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
     },
     {
    "id": 5678,
    "category": {
    "id": 0,
    "name": "Dog"
     },
    "name": "Hero",
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
     

#### Java
The following is an example of a successful  response with status **available**:

    [
     { 
     "id": 1111, 
     "category": 
      { 
        "id": 1111, 
        "name": "fish" 
       }, 
       "name": "Nibbles",
        "photoUrls": [ "<string>" ], 
        "tags": 
        [ 
        { 
        "id": 1111, 
        "name": "<string>" 
        } 
        ], 
        "status": "available" 
        } 
        ]


<!--stackedit_data:
eyJwcm9wZXJ0aWVzIjoidGl0bGU6IFBldFN0b3JlXG5hdXRob3
I6IFRydXB0aVxuc3RhdHVzOiBGcnN0IGRyYWZ0XG5kYXRlOiAy
Mi0wMy0yMDI0XG4iLCJoaXN0b3J5IjpbMjExMzQyMDE4MywtNj
Y3MTY2NTk2XX0=
-->