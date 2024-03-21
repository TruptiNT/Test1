
# Get List of Pets

This section describes the procedure to fetch a list of pets from the  [Swagger Pet store API](https://petstore.swagger.io/) through API interaction.

#### Endpoint
       GET /pet/findByStatus

#### Description
Finds pets by status.
Multiple status values can be provided with comma separated strings.
For this sample, you can use the API key `special-key` to test the authorization filters.

#### Parameters

| Name|Description|Type  |Default|
|--------|-------------------------------------------------------------------------------------------|------|------------|
| status |Status values that need to be considered for filter (values are: available, pending, sold). The field is mandatory |query | available


### Request
https://petstore.swagger.io/v2/pet/findByStatus?status='status'

#### Example Request
Request URL to find pets with the status **available**: 
https://petstore.swagger.io/v2/pet/findByStatus?status=available


### Response

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
#### Response Content Type
-   `application/xml`  
-   `application/json`
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTExNjQyMzk0OTAsLTE2MzUyMDM4NjgsMT
Q4MDkxMjQ5NSwtMTExMTU1ODMyMSwxMTA1NzEwMDc2LDE3NzM0
NDM2ODYsMTQ1MDAxMTg2OF19
-->