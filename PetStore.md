

# Fetch a List of Pets

This section describes the procedure to fetch a list of pets from the Swagger [Pet store API](https://petstore.swagger.io/) through API interaction.

#### Endpoint
       GET /pet/findByStatus

#### Description
Finds pets by status.
Multiple status values can be provided with comma separated strings.

#### Parameters

| Name|Description|Type  |Default|
|--------|-------------------------------------------------------------------------------------------|------|------------|
| *status |Status values that need to be considered for filter (values are: available, pending, sold). The field is mandatory |query | available


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

> Written with [StackEdit](https://stackedit.io/).

<!--stackedit_data:
eyJwcm9wZXJ0aWVzIjoidGl0bGU6IFBldFN0b3JlXG5hdXRob3
I6IFRydXB0aVxuc3RhdHVzOiBGcnN0IGRyYWZ0XG5kYXRlOiAy
Mi0wMy0yMDI0XG4iLCJoaXN0b3J5IjpbLTE0MzcwNzk2MzQsOD
E2NTAyNDA2XX0=
-->