<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>PetStore</title>
  <link rel="stylesheet" href="https://stackedit.io/style.css" />
</head>

<body class="stackedit">
  <div class="stackedit__html">


  
  
  <title>PetStore</title>
  


  <div class="stackedit__html"><p>Get List of PetsThis section describes the procedure to fetch a list of pets from the  <a href="https://petstore.swagger.io/">Swagger Pet store API</a> through API interaction.</p>
</div><h3 id="descriptionfinds-pets-by-status.br">DescriptionFinds pets by status.<br></h3>
<p>Multiple status values can be provided with comma separated strings.<br><br>
For this sample, use the API key <code>special-key</code> to test the authorization filters.</p>
<h3 id="endpoint">Endpoint</h3>
<pre><code>   GET /pet/findByStatus
</code></pre>
<h3 id="parameters">Parameters</h3>
<table>
<thead>
<tr>
<th>Name</th>
<th>Description
</th><th>Type</th>
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
</table><h4 id="example-requesth4">4 id="examplerequesth4"&gt;Example Request</h4>
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
</h4><h3 id="response">Response</h3>
<h4 id="response-codes">Response Codes</h4>| HTTP Code       |Description    }<br>
|<br>
|--------------|-------------------------------|<br>
|200    
||Successful operation
|400           |Invalid Status codeExample Response


</div>
</body>

</html>
