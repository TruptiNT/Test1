
# Get List of Pets

This section describes the procedure to fetch a list of pets from the  [Swagger Pet store API](https://petstore.swagger.io/) through API interaction.

### Description
Finds pets by status.
Multiple status values can be provided with comma separated strings.
For this sample, use the API key `special-key` to test the authorization filters.

### Endpoint
       GET /pet/findByStatus

### Parameters

| Name|Description|Type  |Default|
|--------|-------------------------------------------------------------------------------------------|------|------------|
| status |Status values that need to be considered for filter (values are: available, pending, sold). The field is mandatory |query | available


### Request

#### curl

     curl -X 'GET' \
          'https://petstore.swagger.io/v2/pet/findByStatus?status=available' \
          -H 'accept: application/xml
          
   ###

#### Java
// This code sample uses the 'Unirest' library: 
// http://unirest.io/java.html 

    HttpResponse<String> response = Unirest.get("https://petstore.swagger.io/v2/pet/findByStatus") .header("Accept", "application/xml") .queryString("status", "{status}") .asString(); System.out.println(response.getBody());


#### Example Request
Request URL to find pets with the status **available**: 
https://petstore.swagger.io/v2/pet/findByStatus?status=available

### Response
#### Response Codes

| HTTP Code       |Description                          |           
|--------------|-------------------------------|
|200           |Successful operation   
|400           |Invalid Status code

#### Example Response
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

he following is an example of a successful  response with status **available** in ***Java***

      `[ 
       { 
       "id": 2154, 
       "category": { "id": 2154, "name": "<string>" }, 
       "name": "doggie", 
       "photoUrls": [ "<string>" ], 
       "tags": 
         [ 
          { 
           "id": 2154, 
           "name": "<string>" 
           } 
          ], 
          "status": "available" 
         } 
        ]` 


#### Response Content Type
-   `application/xml`  
-   `application/json`


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEwMjg2ODAxMzQsLTExNjQyMzk0OTAsLT
E2MzUyMDM4NjgsMTQ4MDkxMjQ5NSwtMTExMTU1ODMyMSwxMTA1
NzEwMDc2LDE3NzM0NDM2ODYsMTQ1MDAxMTg2OF19
-->