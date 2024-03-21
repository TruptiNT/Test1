Get List of PetsThis section describes the procedure to fetch a list of pets from the  <a href="https://petstore.swagger.io/">Swagger Pet store API</a> through API interaction.</p>

### Description
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
</table><h4 id="example-requesth4">Example Request</h4>
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
<h4 id="response-codes">Response Codes</h4>
<p>| HTTP Code       |Description    }<br>
|<br>
|--------------|-------------------------------|<br>
|200           |Successful operation<br>
|400           |Invalid Status codeExample Response</p>
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
   "photoUrls": [ "&lt;</code></pre><p></p>
<h4 id="response-content-type">Response Content Type</h4>
<ul>
<li><code>application/xml</code></li>
<li><code>application/json</code></li>
</ul>



</div>
</body>

</html>
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTMzOTkzNDU5MV19
-->