<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>PetStore</title>
  <link rel="stylesheet" href="https://stackedit.io/style.css" />
</head>

<body class="stackedit">
  <div class="stackedit__html"><h1 id="get-list-of-pets">Get List of Pets</h1>
<p>This section describes the procedure to fetch a list of pets from the  <a href="https://petstore.swagger.io/">Swagger Pet store API</a> through API interaction.</p>
<h3 id="description">Description</h3>
<p>Finds pets by status.<br>
Multiple status values can be provided with comma separated strings.<br>
For this sample, use the API key <code>special-key</code> to test the authorization filters.</p>
<h3 id="endpoint">Endpoint</h3>
<pre><code>   GET /pet/findByStatus
</code></pre>
<h3 id="parameters">Parameters</h3>

<table>
<thead>
<tr>
<th>Name</th>
<th>Description</th>
<th>Type</th>
<th>Default</th>
</tr>
</thead>
<tbody>
<tr>
<td>status</td>
<td>Status values that need to be considered for filter (values are: available, pending, sold). The field is mandatory</td>
<td>query</td>
<td>available</td>
</tr>
</tbody>
</table><h3 id="requestRequest</h3>
<h4 id="curl">curl</h4>
<pre><code> curl -X 'GET' \
      'https://petstore.swagger.io/v2/pet/findByStatus?statusavailable' \
      -H 'accept: application/xml
</code></pre>
<h4 id="java">Java</h4>
<p>          
// This code sample uses the ‘Unirest library:<br>
// <a href="http://unirest.io/java.html">http://unirest.io/java.html</a></p>
<pre><code>HttpResponse&lt;<String&gt;> response = Unirest.get("https://petstore.swagger.io/v2/pet/findByStatus") .header("Accept", "application/xml") .queryString("status", "{status}") .asString(); System.out.println(response.getBody());
</code></pre>
<h4 id="example-request">

#### Example Request</h4>
<p>
Request URL to find pets with the status <strong>**available</strong>:<br>
<a href="https://petstore.swagger.io/v2/pet/findByStatus?status=available">https://petstore.swagger.io/v2/pet/findByStatus?status=available</a></p>
<h3 id="response">Response</h3>
<h4 id="response-codes">Response Codes</h4>

<table>
<thead>
<tr>
<th>HTTP Code</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>200</td>
<td>Successful operation</td>
</tr>
<tr>
<td>400</td>
<td>Invalid Status code</td>
</tr>
</tbody>
</table><h4 id="example-response">**: 
https://petstore.swagger.io/v2/pet/findByStatus?status=available

### Response
#### Response Codes

| HTTP Code       |Description    } 
                 |           
|--------------|-------------------------------|
|200           |Successful operation   
|400           |Invalid Status codeExample Response</h4>
<p>
The following is an example of a successful  response with status <strong>**available</strong>:</p>
<pre><code>{
"id": 1234,
"category": {
"id": 0,
"name": "Dog"
 "name": "Zero",
"photoUrls": [
 "strin"
 ],
 "tags": [
  "id": 0,
 "name": "string"
 }
],
 }
</code></pre>
<p>he following is an example of a successful  response with status <strong>**available</strong> in <em><strong>Java</strong></em></p>
<pre><code>  `[ 
   { 
   "id": 2154, 
   "category": { "id": 2154, "name": "&lt;string" }, 
     "name": "doggie", 
   "photoUrls": [ "&lt;<string&gt;>" ], 
   "tags": 
     [ 
      { 
       "id": 2154, 
       "name": "&lt;<string&gt;" 
       
          ], 
      "status": available" 
     } 
    ]` 
</code></pre>
<h4 id="response-content-type">Response Content Type</h4>
<ul>
<li><code>application/xml</code></li>
<li><code>application/json</code></li>
</ul>
</div>
</body>

</html>
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTk0NTY1MTYzOV19
-->