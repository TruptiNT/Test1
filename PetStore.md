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
  


  <div class="stackedit__html"><h1 id="fetch-a-list-of-pets">Fetch a List of Pets</h1>
<p>This section describes the procedure to fetch a list of pets from the Swagger <a href="https://petstore.swagger.io/">Pet store API</a> through API interaction.</p>
<h4 id="endpoint">Endpoint</h4>
<pre><code>   GET /pet/findByStatus
</code></pre>
<h4 id="description">Description</h4>
<p>Finds pets by status.<br>
Multiple status values can be provided with comma separated strings.</p>
<h4 id="parameters">Parameters</h4>
</div><table>
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
<td>*status</td>
<td>Status values that need to be considered for filter (values are: available, pending, sold). The field is mandatory</td>
<td>query</td>
<td>available</td>
</tr>
</tbody>
</table><h3 id="request">Request</h3>
<p><a href="https://petstore.swagger.io/v2/pet/findByStatus?status='status'">https://petstore.swagger.io/v2/pet/findByStatus?status=‘status’</a></p>
<h4 id="example-request">Example Request</h4>
<p>Request URL to find pets with the status <strong>available</strong>:<br>
<a href="https://petstore.swagger.io/v2/pet/findByStatus?status=available">https://petstore.swagger.io/v2/pet/findByStatus?status=available</a></p>
<h3 id="response">Response</h3>
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
</table><h4 id="example-response">Example Response</h4>
<p>The following is an example of a successful  response with status <strong>available</strong>:</p>
<pre><code>{
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
</code></pre>
<h1 id="publication">Publication</h1>
<p>Publishing in StackEdit makes it simple for you to publish online your files. Once you’re happy with a file, you can publish it to different hosting platforms like <strong>Blogger</strong>, <strong>Dropbox</strong>, <strong>Gist</strong>, <strong>GitHub</strong>, <strong>Google Drive</strong>, <strong>WordPress</strong> and <strong>Zendesk</strong>. With <a href="http://handlebarsjs.com/">Handlebars templates</a>, you have full control over what you export.</p>
<blockquote>
<p>Before starting to publish, you must link an account in the <strong>Publish</strong> sub-menu.</p>
</blockquote>
<h2 id="publish-a-file">Publish a File</h2>
<p>You can publish your file by opening the <strong>Publish</strong> sub-menu and by clicking <strong>Publish to</strong>. For some locations, you can choose between the following formats:</p>
<ul>
<li>Markdown: publish the Markdown text on a website that can interpret it (<strong>GitHub</strong> for instance),</li>
<li>HTML: publish the file converted to HTML via a Handlebars template (on a blog for example).</li>
</ul>
<h2 id="update-a-publication">Update a publication</h2>
<p>After publishing, StackEdit keeps your file linked to that publication which makes it easy for you to re-publish it. Once you have modified your file and you want to update your publication, click on the <strong>Publish now</strong> button in the navigation bar.</p>
<blockquote>
<p><strong>Note:</strong> The <strong>Publish now</strong> button is disabled if your file has not been published yet.</p>
</blockquote>
<h2 id="manage-file-publication">Manage file publication</h2>
<p>Since one file can be published to multiple locations, you can list and manage publish locations by clicking <strong>File publication</strong> in the <strong>Publish</strong> sub-menu. This allows you to list and remove publication locations that are linked to your file.</p>
<h1 id="markdown-extensions">Markdown extensions</h1>
<p>StackEdit extends the standard Markdown syntax by adding extra <strong>Markdown extensions</strong>, providing you with some nice features.</p>
<blockquote>
<p><strong>ProTip:</strong> You can disable any <strong>Markdown extension</strong> in the <strong>File properties</strong> dialog.</p>
</blockquote>
<h2 id="smartypants">SmartyPants</h2>
<p>SmartyPants converts ASCII punctuation characters into “smart” typographic punctuation HTML entities. For example:</p>
<table>
<thead>
<tr>
<th></th>
<th>ASCII</th>
<th>HTML</th>
</tr>
</thead>
<tbody>
<tr>
<td>Single backticks</td>
<td><code>'Isn't this fun?'</code></td>
<td>‘Isn’t this fun?’</td>
</tr>
<tr>
<td>Quotes</td>
<td><code>"Isn't this fun?"</code></td>
<td>“Isn’t this fun?”</td>
</tr>
<tr>
<td>Dashes</td>
<td><code>-- is en-dash, --- is em-dash</code></td>
<td>– is en-dash, — is em-dash</td>
</tr>
</tbody>
</table><h2 id="katex">KaTeX</h2>
<p>You can render LaTeX mathematical expressions using <a href="https://khan.github.io/KaTeX/">KaTeX</a>:</p>
<p>The <em>Gamma function</em> satisfying <span class="katex--inline"><span class="katex"><span class="katex-mathml"><math xmlns="http://www.w3.org/1998/Math/MathML"><semantics><mrow><mi mathvariant="normal">Γ</mi><mo stretchy="false">(</mo><mi>n</mi><mo stretchy="false">)</mo><mo>=</mo><mo stretchy="false">(</mo><mi>n</mi><mtext>−</mtext><mn>1</mn><mo stretchy="false">)</mo><mo stretchy="false">!</mo><mi mathvariant="normal">∀</mi><mi>n</mi><mo>∈</mo><mi>N</mi><mi mathvariant="normal">Γ</mi><mo stretchy="false">(</mo><mi>n</mi><mo stretchy="false">)</mo><mo>=</mo><mo stretchy="false">(</mo><mi>n</mi><mo>−</mo><mn>1</mn><mo stretchy="false">)</mo><mo stretchy="false">!</mo><mspace width="1em"></mspace><mi mathvariant="normal">∀</mi><mi>n</mi><mo>∈</mo><mi mathvariant="double-struck">N</mi><mi mathvariant="normal">Γ</mi><mo stretchy="false">(</mo><mi>n</mi><mo stretchy="false">)</mo><mo>=</mo><mo stretchy="false">(</mo><mi>n</mi><mtext>−</mtext><mn>1</mn><mo stretchy="false">)</mo><mo stretchy="false">!</mo><mi mathvariant="normal">∀</mi><mi>n</mi><mo>∈</mo><mi>N</mi></mrow><annotation encoding="application/x-tex">Γ(n)=(n−1)!∀n∈N\Gamma(n) = (n-1)!\quad\forall n\in\mathbb NΓ(n)=(n−1)!∀n∈N</annotation></semantics></math></span><span class="katex-html" aria-hidden="true"><span class="base"><span class="strut" style="height: 1em; vertical-align: -0.25em;"></span><span class="mord">Γ</span><span class="mopen">(</span><span class="mord mathnormal">n</span><span class="mclose">)</span><span class="mspace" style="margin-right: 0.277778em;"></span><span class="mrel">=</span><span class="mspace" style="margin-right: 0.277778em;"></span></span><span class="base"><span class="strut" style="height: 1em; vertical-align: -0.25em;"></span><span class="mopen">(</span><span class="mord mathnormal">n</span><span class="mord">−1</span><span class="mclose">)!</span><span class="mord">∀</span><span class="mord mathnormal">n</span><span class="mspace" style="margin-right: 0.277778em;"></span><span class="mrel">∈</span><span class="mspace" style="margin-right: 0.277778em;"></span></span><span class="base"><span class="strut" style="height: 1em; vertical-align: -0.25em;"></span><span style="margin-right: 0.10903em;" class="mord mathnormal">N</span><span class="mord">Γ</span><span class="mopen">(</span><span class="mord mathnormal">n</span><span class="mclose">)</span><span class="mspace" style="margin-right: 0.277778em;"></span><span class="mrel">=</span><span class="mspace" style="margin-right: 0.277778em;"></span></span><span class="base"><span class="strut" style="height: 1em; vertical-align: -0.25em;"></span><span class="mopen">(</span><span class="mord mathnormal">n</span><span class="mspace" style="margin-right: 0.222222em;"></span><span class="mbin">−</span><span class="mspace" style="margin-right: 0.222222em;"></span></span><span class="base"><span class="strut" style="height: 1em; vertical-align: -0.25em;"></span><span class="mord">1</span><span class="mclose">)!</span><span class="mspace" style="margin-right: 1em;"></span><span class="mord">∀</span><span class="mord mathnormal">n</span><span class="mspace" style="margin-right: 0.277778em;"></span><span class="mrel">∈</span><span class="mspace" style="margin-right: 0.277778em;"></span></span><span class="base"><span class="strut" style="height: 1em; vertical-align: -0.25em;"></span><span class="mord mathbb">N</span><span class="mord">Γ</span><span class="mopen">(</span><span class="mord mathnormal">n</span><span class="mclose">)</span><span class="mspace" style="margin-right: 0.277778em;"></span><span class="mrel">=</span><span class="mspace" style="margin-right: 0.277778em;"></span></span><span class="base"><span class="strut" style="height: 1em; vertical-align: -0.25em;"></span><span class="mopen">(</span><span class="mord mathnormal">n</span><span class="mord">−1</span><span class="mclose">)!</span><span class="mord">∀</span><span class="mord mathnormal">n</span><span class="mspace" style="margin-right: 0.277778em;"></span><span class="mrel">∈</span><span class="mspace" style="margin-right: 0.277778em;"></span></span><span class="base"><span class="strut" style="height: 0.68333em; vertical-align: 0em;"></span><span style="margin-right: 0.10903em;" class="mord mathnormal">N</span></span></span></span></span> is via the Euler integral</p>
<p><span class="katex--display"><span class="katex-display"><span class="katex"><span class="katex-mathml"><math xmlns="http://www.w3.org/1998/Math/MathML" display="block"><semantics><mrow><mi mathvariant="normal">Γ</mi><mo stretchy="false">(</mo><mi>z</mi><mo stretchy="false">)</mo><mo>=</mo><mo>∫</mo><mn>0</mn><mi mathvariant="normal">∞</mi><mi>t</mi><mi>z</mi><mtext>−</mtext><mn>1</mn><mi>e</mi><mtext>−</mtext><mi>t</mi><mi>d</mi><mi>t</mi><mtext> </mtext><mi mathvariant="normal">.</mi><mi mathvariant="normal">Γ</mi><mo stretchy="false">(</mo><mi>z</mi><mo stretchy="false">)</mo><mo>=</mo><msubsup><mo>∫</mo><mn>0</mn><mi mathvariant="normal">∞</mi></msubsup><msup><mi>t</mi><mrow><mi>z</mi><mo>−</mo><mn>1</mn></mrow></msup><msup><mi>e</mi><mrow><mo>−</mo><mi>t</mi></mrow></msup><mi>d</mi><mi>t</mi> <mi mathvariant="normal">.</mi><mi mathvariant="normal">Γ</mi><mo stretchy="false">(</mo><mi>z</mi><mo stretchy="false">)</mo><mo>=</mo><mo>∫</mo><mn>0</mn><mi mathvariant="normal">∞</mi><mtext>​</mtext><mi>t</mi><mi>z</mi><mtext>−</mtext><mn>1</mn><mi>e</mi><mtext>−</mtext><mi>t</mi><mi>d</mi><mi>t</mi><mi mathvariant="normal">.</mi></mrow><annotation encoding="application/x-tex">Γ(z)=∫0∞tz−1e−tdt .
\Gamma(z) = \int_0^\infty t^{z-1}e^{-t}dt\,.
Γ(z)=∫0∞​tz−1e−tdt.</annotation></semantics></math></span><span class="katex-html" aria-hidden="true"><span class="base"><span class="strut" style="height: 1em; vertical-align: -0.25em;"></span><span class="mord">Γ</span><span class="mopen">(</span><span style="margin-right: 0.04398em;" class="mord mathnormal">z</span><span class="mclose">)</span><span class="mspace" style="margin-right: 0.277778em;"></span><span class="mrel">=</span><span class="mspace" style="margin-right: 0.277778em;"></span></span><span class="base"><span class="strut" style="height: 2.22225em; vertical-align: -0.86225em;"></span><span style="margin-right: 0.44445em; position: relative; top: -0.001125em;" class="mop op-symbol large-op">∫</span><span class="mspace" style="margin-right: 0.166667em;"></span><span class="mord">0∞</span><span class="mord mathnormal">t</span><span style="margin-right: 0.04398em;" class="mord mathnormal">z</span><span class="mord">−1</span><span class="mord mathnormal">e</span><span class="mord">−</span><span class="mord mathnormal">t</span><span class="mord mathnormal">d</span><span class="mord mathnormal">t</span><span class="mord"> .Γ</span><span class="mopen">(</span><span style="margin-right: 0.04398em;" class="mord mathnormal">z</span><span class="mclose">)</span><span class="mspace" style="margin-right: 0.277778em;"></span><span class="mrel">=</span><span class="mspace" style="margin-right: 0.277778em;"></span></span><span class="base"><span class="strut" style="height: 2.32624em; vertical-align: -0.91195em;"></span><span class="mop"><span style="margin-right: 0.44445em; position: relative; top: -0.001125em;" class="mop op-symbol large-op">∫</span><span class="msupsub"><span class="vlist-t vlist-t2"><span class="vlist-r"><span class="vlist" style="height: 1.41429em;"><span class="" style="top: -1.78805em; margin-left: -0.44445em; margin-right: 0.05em;"><span class="pstrut" style="height: 2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mtight">0</span></span></span><span class="" style="top: -3.8129em; margin-right: 0.05em;"><span class="pstrut" style="height: 2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mtight">∞</span></span></span></span><span class="vlist-s">​</span></span><span class="vlist-r"><span class="vlist" style="height: 0.91195em;"><span class=""></span></span></span></span></span></span><span class="mspace" style="margin-right: 0.166667em;"></span><span class="mord"><span class="mord mathnormal">t</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height: 0.864108em;"><span class="" style="top: -3.113em; margin-right: 0.05em;"><span class="pstrut" style="height: 2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mtight"><span style="margin-right: 0.04398em;" class="mord mathnormal mtight">z</span><span class="mbin mtight">−</span><span class="mord mtight">1</span></span></span></span></span></span></span></span></span><span class="mord"><span class="mord mathnormal">e</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height: 0.843556em;"><span class="" style="top: -3.113em; margin-right: 0.05em;"><span class="pstrut" style="height: 2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mtight"><span class="mord mtight">−</span><span class="mord mathnormal mtight">t</span></span></span></span></span></span></span></span></span><span class="mord mathnormal">d</span><span class="mord mathnormal">t</span><span class="mspace" style="margin-right: 0.166667em;"></span><span class="mord">.Γ</span><span class="mopen">(</span><span style="margin-right: 0.04398em;" class="mord mathnormal">z</span><span class="mclose">)</span><span class="mspace" style="margin-right: 0.277778em;"></span><span class="mrel">=</span><span class="mspace" style="margin-right: 0.277778em;"></span></span><span class="base"><span class="strut" style="height: 2.22225em; vertical-align: -0.86225em;"></span><span style="margin-right: 0.44445em; position: relative; top: -0.001125em;" class="mop op-symbol large-op">∫</span><span class="mspace" style="margin-right: 0.166667em;"></span><span class="mord">0∞​</span><span class="mord mathnormal">t</span><span style="margin-right: 0.04398em;" class="mord mathnormal">z</span><span class="mord">−1</span><span class="mord mathnormal">e</span><span class="mord">−</span><span class="mord mathnormal">t</span><span class="mord mathnormal">d</span><span class="mord mathnormal">t</span><span class="mord">.</span></span></span></span></span></span></p>
<blockquote>
<p>You can find more information about <strong>LaTeX</strong> mathematical expressions <a href="http://meta.math.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference">here</a>.</p>
</blockquote>
<h2 id="uml-diagrams">UML diagrams</h2>
<p>You can render UML diagrams using <a href="https://mermaidjs.github.io/">Mermaid</a>. For example, this will produce a sequence diagram:</p>
<pre class=" language-mermaid"><svg id="mermaid-svg-XoO2juiO02npuUmh" width="100%" xmlns="http://www.w3.org/2000/svg" height="553" viewBox="-50 -10 814 553"><g><g class="output"><g class="clusters"></g><g class="edgePaths"><g class="edgePath LS-A LE-B" id="L-A-B"><path class="path" d="M109.67378624267701,67.60832977294922L170.0749969482422,38.85832977294922L246.16666412353516,38.85832977294922" marker-end="url(https://stackedit.io/app#arrowhead13)"></path><defs><marker id="arrowhead13" viewBox="0 0 10 10" refX="9" refY="5" markerUnits="strokeWidth" markerWidth="8" markerHeight="6" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowheadPath"></path></marker></defs></g><g class="edgePath LS-A LE-C" id="L-A-C"><path class="path" d="M109.67378624267701,114.32498931884766L170.0749969482422,143.07498931884766L226.9499969482422,143.07498931884766" marker-end="url(https://stackedit.io/app#arrowhead14)"></path><defs><marker id="arrowhead14" viewBox="0 0 10 10" refX="9" refY="5" markerUnits="strokeWidth" markerWidth="8" markerHeight="6" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowheadPath"></path></marker></defs></g><g class="edgePath LS-B LE-D" id="L-B-D"><path class="path" d="M307.8833236694336,38.85832977294922L352.09999084472656,38.85832977294922L400.1574218001457,68.90923011635829" marker-end="url(https://stackedit.io/app#arrowhead15)"></path><defs><marker id="arrowhead15" viewBox="0 0 10 10" refX="9" refY="5" markerUnits="strokeWidth" markerWidth="8" markerHeight="6" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowheadPath"></path></marker></defs></g><g class="edgePath LS-C LE-D" id="L-C-D"><path class="path" d="M327.09999084472656,143.07498931884766L352.09999084472656,143.07498931884766L400.1574199179397,114.02409014499051" marker-end="url(https://stackedit.io/app#arrowhead16)"></path><defs><marker id="arrowhead16" viewBox="0 0 10 10" refX="9" refY="5" markerUnits="strokeWidth" markerWidth="8" markerHeight="6" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowheadPath"></path></marker></defs></g></g><g class="edgeLabels"><g class="edgeLabel" transform="translate(170.0749969482422,38.85832977294922)"><g transform="translate(-31.875,-13.358329772949219)" class="label"><rect rx="0" ry="0" width="63.75" height="26.716659545898438"></rect><div xmlns="http://www.w3.org/1999/xhtml"><span id="L-L-A-B" class="edgeLabel L-LS-A' L-LE-B">Link text</span></div></g></g><g class="edgeLabel" transform=""><g transform="translate(0,0)" class="label"><rect rx="0" ry="0" width="0" height="0"></rect><div xmlns="http://www.w3.org/1999/xhtml"><span id="L-L-A-C" class="edgeLabel L-LS-A' L-LE-C"></span></div></g></g><g class="edgeLabel" transform=""><g transform="translate(0,0)" class="label"><rect rx="0" ry="0" width="0" height="0"></rect><div xmlns="http://www.w3.org/1999/xhtml"><span id="L-L-B-D" class="edgeLabel L-LS-B' L-LE-D"></span></div></g></g><g class="edgeLabel" transform=""><g transform="translate(0,0)" class="label"><rect rx="0" ry="0" width="0" height="0"></rect><div xmlns="http://www.w3.org/1999/xhtml"><span id="L-L-C-D" class="edgeLabel L-LS-C' L-LE-D"></span></div></g></g></g><g class="nodes"><g class="node default" id="flowchart-A-56" transform="translate(60.599998474121094,90.96665954589844)"><rect rx="0" ry="0" x="-52.599998474121094" y="-23.35832977294922" width="105.19999694824219" height="46.71665954589844" class="label-container"></rect><g class="label" transform="translate(0,0)"><g transform="translate(-42.599998474121094,-13.358329772949219)"><div xmlns="http://www.w3.org/1999/xhtml">Square Rect</div></g></g></g><g class="node default" id="flowchart-B-57" transform="translate(277.0249938964844,38.85832977294922)"><circle x="-30.85832977294922" y="-23.35832977294922" r="30.85832977294922" class="label-container"></circle><g class="label" transform="translate(0,0)"><g transform="translate(-20.85832977294922,-13.358329772949219)"><div xmlns="http://www.w3.org/1999/xhtml">Circle</div></g></g></g><g class="node default" id="flowchart-C-59" transform="translate(277.0249938964844,143.07498931884766)"><rect rx="5" ry="5" x="-50.07499694824219" y="-23.35832977294922" width="100.14999389648438" height="46.71665954589844" class="label-container"></rect><g class="label" transform="translate(0,0)"><g transform="translate(-40.07499694824219,-13.358329772949219)"><div xmlns="http://www.w3.org/1999/xhtml">Round Rect</div></g></g></g><g class="node default" id="flowchart-D-61" transform="translate(435.9599838256836,90.96665954589844)"><polygon points="58.85999450683594,0 117.71998901367188,-58.85999450683594 58.85999450683594,-117.71998901367188 0,-58.85999450683594" transform="translate(-58.85999450683594,58.85999450683594)" class="label-container"></polygon><g class="label" transform="translate(0,0)"><g transform="translate(-32.041664123535156,-13.358329772949219)"><div xmlns="http://www.w3.org/1999/xhtml">Rhombus</div></g></g></g></g></g></g></svg></pre>
<blockquote>
<p>Written with <a href="https://stackedit.io/">StackEdit</a>.</p>
</blockquote>



# Fetch a List of Pets
<p>This section describes the procedure to fetch a list of pets from the Swagger <a href="https://petstore.swagger.io/">Pet store API</a> through API interaction.</p>
<h4 id="endpoint">Endpoint</h4>
<pre><code>   GET /pet/findByStatus
</code></pre>
<h4 id="description">Description</h4>
<p>Finds pets by status.<br>
Multiple status values can be provided with comma separated strings.</p>
<h4 id="parameters">Parameters</h4>

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
<td>*status</td>
<td>Status values that need to be considered for filter (values are: available, pending, sold). The field is mandatory</td>
<td>query</td>
<td>available</td>
</tr>
</tbody>
</table><h3 id="request">Request</h3>
<p><a href="https://petstore.swagger.io/v2/pet/findByStatus?status='status'">https://petstore.swagger.io/v2/pet/findByStatus?status=‘status’</a></p>
<h4 id="example-request">Example Request</h4>
<p>Request URL to find pets with the status <strong>available</strong>:<br>
<a href="https://petstore.swagger.io/v2/pet/findByStatus?status=available">https://petstore.swagger.io/v2/pet/findByStatus?status=available</a></p>
<h3 id="response">Response</h3>

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
</table><h4 id="example-response">Example Response</h4>
<p>The following is an example of a successful  response with status <strong>available</strong>:</p>
<pre><code>{
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
</code></pre>
<h1 id="publication">Publication</h1>
<p>Publishing in StackEdit makes it simple for you to publish online your files. Once you’re happy with a file, you can publish it to different hosting platforms like <strong>Blogger</strong>, <strong>Dropbox</strong>, <strong>Gist</strong>, <strong>GitHub</strong>, <strong>Google Drive</strong>, <strong>WordPress</strong> and <strong>Zendesk</strong>. With <a href="http://handlebarsjs.com/">Handlebars templates</a>, you have full control over what you export.</p>
<blockquote>
<p>Before starting to publish, you must link an account in the <strong>Publish</strong> sub-menu.</p>
</blockquote>
<h2 id="publish-a-file">Publish a File</h2>
<p>You can publish your file by opening the <strong>Publish</strong> sub-menu and by clicking <strong>Publish to</strong>. For some locations, you can choose between the following formats:</p>
<ul>
<li>Markdown: publish the Markdown text on a website that can interpret it (<strong>GitHub</strong> for instance),</li>
<li>HTML: publish the file converted to HTML via a Handlebars template (on a blog for example).</li>
</ul>
<h2 id="update-a-publication">Update a publication</h2>
<p>After publishing, StackEdit keeps your file linked to that publication which makes it easy for you to re-publish it. Once you have modified your file and you want to update your publication, click on the <strong>Publish now</strong> button in the navigation bar.</p>
<blockquote>
<p><strong>Note:</strong> The <strong>Publish now</strong> button is disabled if your file has not been published yet.</p>
</blockquote>
<h2 id="manage-file-publication">Manage file publication</h2>
<p>Since one file can be published to multiple locations, you can list and manage publish locations by clicking <strong>File publication</strong> in the <strong>Publish</strong> sub-menu. This allows you to list and remove publication locations that are linked to your file.</p>
<h1 id="markdown-extensions">Markdown extensions</h1>
<p>StackEdit extends the standard Markdown syntax by adding extra <strong>Markdown extensions</strong>, providing you with some nice features.</p>
<blockquote>
<p><strong>ProTip:</strong> You can disable any <strong>Markdown extension</strong> in the <strong>File properties</strong> dialog.</p>
</blockquote>
<h2 id="smartypants">SmartyPants</h2>
<p>SmartyPants converts ASCII punctuation characters into “smart” typographic punctuation HTML entities. For example:</p>

<table>
<thead>
<tr>
<th></th>
<th>ASCII</th>
<th>HTML</th>
</tr>
</thead>
<tbody>
<tr>
<td>Single backticks</td>
<td><code>'Isn't this fun?'</code></td>
<td>‘Isn’t this fun?’</td>
</tr>
<tr>
<td>Quotes</td>
<td><code>"Isn't this fun?"</code></td>
<td>“Isn’t this fun?”</td>
</tr>
<tr>
<td>Dashes</td>
<td><code>-- is en-dash, --- is em-dash</code></td>
<td>– is en-dash, — is em-dash</td>
</tr>
</tbody>
</table><h2 id="katex">KaTeX</h2>
<p>You can render LaTeX mathematical expressions using <a href="https://khan.github.io/KaTeX/">KaTeX</a>:</p>
<p>The <em>Gamma function</em> satisfying <span class="katex--inline"><span class="katex"><span class="katex-mathml"><math xmlns="http://www.w3.org/1998/Math/MathML"><semantics><mrow><mi mathvariant="normal">Γ</mi><mo stretchy="false">(</mo><mi>n</mi><mo stretchy="false">)</mo><mo>=</mo><mo stretchy="false">(</mo><mi>n</mi><mo>−</mo><mn>1</mn><mo stretchy="false">)</mo><mo stretchy="false">!</mo><mspace width="1em"></mspace><mi mathvariant="normal">∀</mi><mi>n</mi><mo>∈</mo><mi mathvariant="double-struck">N</mi></mrow><annotation encoding="application/x-tex">\Gamma(n) = (n-1)!\quad\forall n\in\mathbb N</annotation></semantics></math></span><span class="katex-html" aria-hidden="true"><span class="base"><span class="strut" style="height: 1em; vertical-align: -0.25em;"></span><span class="mord">Γ</span><span class="mopen">(</span><span class="mord mathnormal">n</span><span class="mclose">)</span><span class="mspace" style="margin-right: 0.277778em;"></span><span class="mrel">=</span><span class="mspace" style="margin-right: 0.277778em;"></span></span><span class="base"><span class="strut" style="height: 1em; vertical-align: -0.25em;"></span><span class="mopen">(</span><span class="mord mathnormal">n</span><span class="mspace" style="margin-right: 0.222222em;"></span><span class="mbin">−</span><span class="mspace" style="margin-right: 0.222222em;"></span></span><span class="base"><span class="strut" style="height: 1em; vertical-align: -0.25em;"></span><span class="mord">1</span><span class="mclose">)!</span><span class="mspace" style="margin-right: 1em;"></span><span class="mord">∀</span><span class="mord mathnormal">n</span><span class="mspace" style="margin-right: 0.277778em;"></span><span class="mrel">∈</span><span class="mspace" style="margin-right: 0.277778em;"></span></span><span class="base"><span class="strut" style="height: 0.68889em; vertical-align: 0em;"></span><span class="mord mathbb">N</span></span></span></span></span> is via the Euler integral</p>
<p><span class="katex--display"><span class="katex-display"><span class="katex"><span class="katex-mathml"><math xmlns="http://www.w3.org/1998/Math/MathML" display="block"><semantics><mrow><mi mathvariant="normal">Γ</mi><mo stretchy="false">(</mo><mi>z</mi><mo stretchy="false">)</mo><mo>=</mo><msubsup><mo>∫</mo><mn>0</mn><mi mathvariant="normal">∞</mi></msubsup><msup><mi>t</mi><mrow><mi>z</mi><mo>−</mo><mn>1</mn></mrow></msup><msup><mi>e</mi><mrow><mo>−</mo><mi>t</mi></mrow></msup><mi>d</mi><mi>t</mi> <mi mathvariant="normal">.</mi></mrow><annotation encoding="application/x-tex">
\Gamma(z) = \int_0^\infty t^{z-1}e^{-t}dt\,.
</annotation></semantics></math></span><span class="katex-html" aria-hidden="true"><span class="base"><span class="strut" style="height: 1em; vertical-align: -0.25em;"></span><span class="mord">Γ</span><span class="mopen">(</span><span style="margin-right: 0.04398em;" class="mord mathnormal">z</span><span class="mclose">)</span><span class="mspace" style="margin-right: 0.277778em;"></span><span class="mrel">=</span><span class="mspace" style="margin-right: 0.277778em;"></span></span><span class="base"><span class="strut" style="height: 2.32624em; vertical-align: -0.91195em;"></span><span class="mop"><span style="margin-right: 0.44445em; position: relative; top: -0.001125em;" class="mop op-symbol large-op">∫</span><span class="msupsub"><span class="vlist-t vlist-t2"><span class="vlist-r"><span class="vlist" style="height: 1.41429em;"><span class="" style="top: -1.78805em; margin-left: -0.44445em; margin-right: 0.05em;"><span class="pstrut" style="height: 2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mtight">0</span></span></span><span class="" style="top: -3.8129em; margin-right: 0.05em;"><span class="pstrut" style="height: 2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mtight">∞</span></span></span></span><span class="vlist-s">​</span></span><span class="vlist-r"><span class="vlist" style="height: 0.91195em;"><span class=""></span></span></span></span></span></span><span class="mspace" style="margin-right: 0.166667em;"></span><span class="mord"><span class="mord mathnormal">t</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height: 0.864108em;"><span class="" style="top: -3.113em; margin-right: 0.05em;"><span class="pstrut" style="height: 2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mtight"><span style="margin-right: 0.04398em;" class="mord mathnormal mtight">z</span><span class="mbin mtight">−</span><span class="mord mtight">1</span></span></span></span></span></span></span></span></span><span class="mord"><span class="mord mathnormal">e</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height: 0.843556em;"><span class="" style="top: -3.113em; margin-right: 0.05em;"><span class="pstrut" style="height: 2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mtight"><span class="mord mtight">−</span><span class="mord mathnormal mtight">t</span></span></span></span></span></span></span></span></span><span class="mord mathnormal">d</span><span class="mord mathnormal">t</span><span class="mspace" style="margin-right: 0.166667em;"></span><span class="mord">.</span></span></span></span></span></span></p>
<blockquote>
<p>You can find more information about <strong>LaTeX</strong> mathematical expressions <a href="http://meta.math.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference">here</a>.</p>
</blockquote>
<h2 id="uml-diagrams">UML diagrams</h2>
<p>You can render UML diagrams using <a href="https://mermaidjs.github.io/">Mermaid</a>. For example, this will produce a sequence diagram:</p>
<pre class=" language-mermaid"><svg id="mermaid-svg-dvS1Mm08zy0zo8hD" width="100%" xmlns="http://www.w3.org/2000/svg" height="553" style="max-width: 814px;" viewBox="-50 -10 814 553"><style>#mermaid-svg-dvS1Mm08zy0zo8hD{font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:16px;fill:#000000;}#mermaid-svg-dvS1Mm08zy0zo8hD .error-icon{fill:#552222;}#mermaid-svg-dvS1Mm08zy0zo8hD .error-text{fill:#552222;stroke:#552222;}#mermaid-svg-dvS1Mm08zy0zo8hD .edge-thickness-normal{stroke-width:2px;}#mermaid-svg-dvS1Mm08zy0zo8hD .edge-thickness-thick{stroke-width:3.5px;}#mermaid-svg-dvS1Mm08zy0zo8hD .edge-pattern-solid{stroke-dasharray:0;}#mermaid-svg-dvS1Mm08zy0zo8hD .edge-pattern-dashed{stroke-dasharray:3;}#mermaid-svg-dvS1Mm08zy0zo8hD .edge-pattern-dotted{stroke-dasharray:2;}#mermaid-svg-dvS1Mm08zy0zo8hD .marker{fill:#666;stroke:#666;}#mermaid-svg-dvS1Mm08zy0zo8hD .marker.cross{stroke:#666;}#mermaid-svg-dvS1Mm08zy0zo8hD svg{font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:16px;}#mermaid-svg-dvS1Mm08zy0zo8hD .actor{stroke:hsl(0,0%,83%);fill:#eee;}#mermaid-svg-dvS1Mm08zy0zo8hD text.actor > tspan{fill:#333;stroke:none;}#mermaid-svg-dvS1Mm08zy0zo8hD .actor-line{stroke:#666;}#mermaid-svg-dvS1Mm08zy0zo8hD .messageLine0{stroke-width:1.5;stroke-dasharray:none;stroke:#333;}#mermaid-svg-dvS1Mm08zy0zo8hD .messageLine1{stroke-width:1.5;stroke-dasharray:2,2;stroke:#333;}#mermaid-svg-dvS1Mm08zy0zo8hD #arrowhead path{fill:#333;stroke:#333;}#mermaid-svg-dvS1Mm08zy0zo8hD .sequenceNumber{fill:white;}#mermaid-svg-dvS1Mm08zy0zo8hD #sequencenumber{fill:#333;}#mermaid-svg-dvS1Mm08zy0zo8hD #crosshead path{fill:#333;stroke:#333;}#mermaid-svg-dvS1Mm08zy0zo8hD .messageText{fill:#333;stroke:#333;}#mermaid-svg-dvS1Mm08zy0zo8hD .labelBox{stroke:hsl(0,0%,83%);fill:#eee;}#mermaid-svg-dvS1Mm08zy0zo8hD .labelText,#mermaid-svg-dvS1Mm08zy0zo8hD .labelText > tspan{fill:#333;stroke:none;}#mermaid-svg-dvS1Mm08zy0zo8hD .loopText,#mermaid-svg-dvS1Mm08zy0zo8hD .loopText > tspan{fill:#333;stroke:none;}#mermaid-svg-dvS1Mm08zy0zo8hD .loopLine{stroke-width:2px;stroke-dasharray:2,2;stroke:hsl(0,0%,83%);fill:hsl(0,0%,83%);}#mermaid-svg-dvS1Mm08zy0zo8hD .note{stroke:hsl(60,100%,23.3333333333%);fill:#ffa;}#mermaid-svg-dvS1Mm08zy0zo8hD .noteText,#mermaid-svg-dvS1Mm08zy0zo8hD .noteText > tspan{fill:#333;stroke:none;}#mermaid-svg-dvS1Mm08zy0zo8hD .activation0{fill:#f4f4f4;stroke:#666;}#mermaid-svg-dvS1Mm08zy0zo8hD .activation1{fill:#f4f4f4;stroke:#666;}#mermaid-svg-dvS1Mm08zy0zo8hD .activation2{fill:#f4f4f4;stroke:#666;}#mermaid-svg-dvS1Mm08zy0zo8hD:root{--mermaid-font-family:"trebuchet ms",verdana,arial,sans-serif;}#mermaid-svg-dvS1Mm08zy0zo8hD sequence{fill:apa;}</style><g></g><g><line id="actor12" x1="75" y1="5" x2="75" y2="542" class="actor-line" stroke-width="0.5px" stroke="#999"></line><rect x="0" y="0" fill="#eaeaea" stroke="#666" width="150" height="65" rx="3" ry="3" class="actor"></rect><text x="75" y="32.5" style="text-anchor: middle; font-weight: 400; font-family: &quot;Open-Sans&quot;, &quot;sans-serif&quot;;" dominant-baseline="central" alignment-baseline="central" class="actor"><tspan x="75" dy="0">Alice</tspan></text></g><g><line id="actor13" x1="318" y1="5" x2="318" y2="542" class="actor-line" stroke-width="0.5px" stroke="#999"></line><rect x="243" y="0" fill="#eaeaea" stroke="#666" width="150" height="65" rx="3" ry="3" class="actor"></rect><text x="318" y="32.5" style="text-anchor: middle; font-weight: 400; font-family: &quot;Open-Sans&quot;, &quot;sans-serif&quot;;" dominant-baseline="central" alignment-baseline="central" class="actor"><tspan x="318" dy="0">Bob</tspan></text></g><g><line id="actor14" x1="539" y1="5" x2="539" y2="542" class="actor-line" stroke-width="0.5px" stroke="#999"></line><rect x="464" y="0" fill="#eaeaea" stroke="#666" width="150" height="65" rx="3" ry="3" class="actor"></rect><text x="539" y="32.5" style="text-anchor: middle; font-weight: 400; font-family: &quot;Open-Sans&quot;, &quot;sans-serif&quot;;" dominant-baseline="central" alignment-baseline="central" class="actor"><tspan x="539" dy="0">John</tspan></text></g><defs><marker id="arrowhead" refX="9" refY="5" markerUnits="userSpaceOnUse" markerWidth="12" markerHeight="12" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z"></path></marker></defs><defs><marker id="crosshead" markerWidth="15" markerHeight="8" orient="auto" refX="16" refY="4"><path fill="black" stroke="#000000" style="stroke-dasharray: 0px, 0px;" stroke-width="1px" d="M 9,2 V 6 L16,4 Z"></path><path fill="none" stroke="#000000" style="stroke-dasharray: 0px, 0px;" stroke-width="1px" d="M 0,1 L 6,7 M 6,1 L 0,7"></path></marker></defs><defs><marker id="filled-head" refX="18" refY="7" markerWidth="20" markerHeight="28" orient="auto"><path d="M 18,7 L9,13 L14,7 L9,1 Z"></path></marker></defs><defs><marker id="sequencenumber" refX="15" refY="15" markerWidth="60" markerHeight="40" orient="auto"><circle cx="15" cy="15" r="6"></circle></marker></defs><text x="197" y="80" text-anchor="middle" dominant-baseline="middle" alignment-baseline="middle" style="font-family: &quot;trebuchet ms&quot;, verdana, arial, sans-serif; font-weight: 400;" class="messageText" dy="1em">Hello Bob, how are you?</text><line x1="75" y1="113" x2="318" y2="113" class="messageLine0" stroke-width="2" stroke="none" style="fill: none;" marker-end="url(#arrowhead)"></line><text x="429" y="128" text-anchor="middle" dominant-baseline="middle" alignment-baseline="middle" style="font-family: &quot;trebuchet ms&quot;, verdana, arial, sans-serif; font-weight: 400;" class="messageText" dy="1em">How about you John?</text><line x1="318" y1="161" x2="539" y2="161" style="stroke-dasharray: 3px, 3px; fill: none;" class="messageLine1" stroke-width="2" stroke="none" marker-end="url(#arrowhead)"></line><text x="197" y="176" text-anchor="middle" dominant-baseline="middle" alignment-baseline="middle" style="font-family: &quot;trebuchet ms&quot;, verdana, arial, sans-serif; font-weight: 400;" class="messageText" dy="1em">I am good thanks!</text><line x1="318" y1="209" x2="75" y2="209" style="stroke-dasharray: 3px, 3px; fill: none;" class="messageLine1" stroke-width="2" stroke="none" marker-end="url(#crosshead)"></line><text x="429" y="224" text-anchor="middle" dominant-baseline="middle" alignment-baseline="middle" style="font-family: &quot;trebuchet ms&quot;, verdana, arial, sans-serif; font-weight: 400;" class="messageText" dy="1em">I am good thanks!</text><line x1="318" y1="257" x2="539" y2="257" class="messageLine0" stroke-width="2" stroke="none" style="fill: none;" marker-end="url(#crosshead)"></line><g><rect x="564" y="267" fill="#EDF2AE" stroke="#666" width="150" height="94" rx="0" ry="0" class="note"></rect><text x="639" y="272" text-anchor="middle" dominant-baseline="middle" alignment-baseline="middle" style="font-family: &quot;trebuchet ms&quot;, verdana, arial, sans-serif; font-weight: 400;" class="noteText" dy="1em"><tspan x="639">Bob thinks a long</tspan></text><text x="639" y="291" text-anchor="middle" dominant-baseline="middle" alignment-baseline="middle" style="font-family: &quot;trebuchet ms&quot;, verdana, arial, sans-serif; font-weight: 400;" class="noteText" dy="1em"><tspan x="639">long time, so long</tspan></text><text x="639" y="309" text-anchor="middle" dominant-baseline="middle" alignment-baseline="middle" style="font-family: &quot;trebuchet ms&quot;, verdana, arial, sans-serif; font-weight: 400;" class="noteText" dy="1em"><tspan x="639">that the text does</tspan></text><text x="639" y="328" text-anchor="middle" dominant-baseline="middle" alignment-baseline="middle" style="font-family: &quot;trebuchet ms&quot;, verdana, arial, sans-serif; font-weight: 400;" class="noteText" dy="1em"><tspan x="639">not fit on a row.</tspan></text></g><text x="197" y="376" text-anchor="middle" dominant-baseline="middle" alignment-baseline="middle" style="font-family: &quot;trebuchet ms&quot;, verdana, arial, sans-serif; font-weight: 400;" class="messageText" dy="1em">Checking with John...</text><line x1="318" y1="409" x2="75" y2="409" style="stroke-dasharray: 3px, 3px; fill: none;" class="messageLine1" stroke-width="2" stroke="none"></line><text x="307" y="424" text-anchor="middle" dominant-baseline="middle" alignment-baseline="middle" style="font-family: &quot;trebuchet ms&quot;, verdana, arial, sans-serif; font-weight: 400;" class="messageText" dy="1em">Yes... John, how are you?</text><line x1="75" y1="457" x2="539" y2="457" class="messageLine0" stroke-width="2" stroke="none" style="fill: none;"></line><g><rect x="0" y="477" fill="#eaeaea" stroke="#666" width="150" height="65" rx="3" ry="3" class="actor"></rect><text x="75" y="509.5" style="text-anchor: middle; font-weight: 400; font-family: &quot;Open-Sans&quot;, &quot;sans-serif&quot;;" dominant-baseline="central" alignment-baseline="central" class="actor"><tspan x="75" dy="0">Alice</tspan></text></g><g><rect x="243" y="477" fill="#eaeaea" stroke="#666" width="150" height="65" rx="3" ry="3" class="actor"></rect><text x="318" y="509.5" style="text-anchor: middle; font-weight: 400; font-family: &quot;Open-Sans&quot;, &quot;sans-serif&quot;;" dominant-baseline="central" alignment-baseline="central" class="actor"><tspan x="318" dy="0">Bob</tspan></text></g><g><rect x="464" y="477" fill="#eaeaea" stroke="#666" width="150" height="65" rx="3" ry="3" class="actor"></rect><text x="539" y="509.5" style="text-anchor: middle; font-weight: 400; font-family: &quot;Open-Sans&quot;, &quot;sans-serif&quot;;" dominant-baseline="central" alignment-baseline="central" class="actor"><tspan x="539" dy="0">John</tspan></text></g></svg></pre>
<p>And this will produce a flow chart:</p>
<pre class=" language-mermaid"><svg id="mermaid-svg-Q9ZeaibDzrjV4bl2" width="100%" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" height="174.43331909179688" style="max-width: 502.82000732421875px;" viewBox="0 0 502.82000732421875 174.43331909179688"><style>#mermaid-svg-Q9ZeaibDzrjV4bl2{font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:16px;fill:#000000;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .error-icon{fill:#552222;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .error-text{fill:#552222;stroke:#552222;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .edge-thickness-normal{stroke-width:2px;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .edge-thickness-thick{stroke-width:3.5px;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .edge-pattern-solid{stroke-dasharray:0;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .edge-pattern-dashed{stroke-dasharray:3;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .edge-pattern-dotted{stroke-dasharray:2;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .marker{fill:#666;stroke:#666;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .marker.cross{stroke:#666;}#mermaid-svg-Q9ZeaibDzrjV4bl2 svg{font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:16px;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .label{font-family:"trebuchet ms",verdana,arial,sans-serif;color:#000000;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .cluster-label text{fill:#333;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .cluster-label span{color:#333;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .label text,#mermaid-svg-Q9ZeaibDzrjV4bl2 span{fill:#000000;color:#000000;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .node rect,#mermaid-svg-Q9ZeaibDzrjV4bl2 .node circle,#mermaid-svg-Q9ZeaibDzrjV4bl2 .node ellipse,#mermaid-svg-Q9ZeaibDzrjV4bl2 .node polygon,#mermaid-svg-Q9ZeaibDzrjV4bl2 .node path{fill:#eee;stroke:#999;stroke-width:1px;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .node .label{text-align:center;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .node.clickable{cursor:pointer;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .arrowheadPath{fill:#333333;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .edgePath .path{stroke:#666;stroke-width:1.5px;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .flowchart-link{stroke:#666;fill:none;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .edgeLabel{background-color:white;text-align:center;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .edgeLabel rect{opacity:0.5;background-color:white;fill:white;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .cluster rect{fill:hsl(210,66.6666666667%,95%);stroke:#26a;stroke-width:1px;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .cluster text{fill:#333;}#mermaid-svg-Q9ZeaibDzrjV4bl2 .cluster span{color:#333;}#mermaid-svg-Q9ZeaibDzrjV4bl2 div.mermaidTooltip{position:absolute;text-align:center;max-width:200px;padding:2px;font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:12px;background:hsl(-160,0%,93.3333333333%);border:1px solid #26a;border-radius:2px;pointer-events:none;z-index:100;}#mermaid-svg-Q9ZeaibDzrjV4bl2:root{--mermaid-font-family:"trebuchet ms",verdana,arial,sans-serif;}#mermaid-svg-Q9ZeaibDzrjV4bl2 flowchart{fill:apa;}</style><g><g class="output"><g class="clusters"></g><g class="edgePaths"><g class="edgePath LS-A LE-B" style="opacity: 1;" id="L-A-B"><path class="path" d="M109.67378624267701,67.60832977294922L170.0749969482422,38.85832977294922L246.16666412353516,38.85832977294922" marker-end="url(https://stackedit.io/app#arrowhead17)" style="fill:none"></path><defs><marker id="arrowhead17" viewBox="0 0 10 10" refX="9" refY="5" markerUnits="strokeWidth" markerWidth="8" markerHeight="6" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowheadPath" style="stroke-width: 1px; stroke-dasharray: 1px, 0px;"></path></marker></defs></g><g class="edgePath LS-A LE-C" style="opacity: 1;" id="L-A-C"><path class="path" d="M109.67378624267701,114.32498931884766L170.0749969482422,143.07498931884766L226.9499969482422,143.07498931884766" marker-end="url(https://stackedit.io/app#arrowhead18)" style="fill:none"></path><defs><marker id="arrowhead18" viewBox="0 0 10 10" refX="9" refY="5" markerUnits="strokeWidth" markerWidth="8" markerHeight="6" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowheadPath" style="stroke-width: 1px; stroke-dasharray: 1px, 0px;"></path></marker></defs></g><g class="edgePath LS-B LE-D" style="opacity: 1;" id="L-B-D"><path class="path" d="M307.8833236694336,38.85832977294922L352.09999084472656,38.85832977294922L400.1574218001457,68.90923011635829" marker-end="url(https://stackedit.io/app#arrowhead19)" style="fill:none"></path><defs><marker id="arrowhead19" viewBox="0 0 10 10" refX="9" refY="5" markerUnits="strokeWidth" markerWidth="8" markerHeight="6" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowheadPath" style="stroke-width: 1px; stroke-dasharray: 1px, 0px;"></path></marker></defs></g><g class="edgePath LS-C LE-D" style="opacity: 1;" id="L-C-D"><path class="path" d="M327.09999084472656,143.07498931884766L352.09999084472656,143.07498931884766L400.1574199179397,114.02409014499051" marker-end="url(https://stackedit.io/app#arrowhead20)" style="fill:none"></path><defs><marker id="arrowhead20" viewBox="0 0 10 10" refX="9" refY="5" markerUnits="strokeWidth" markerWidth="8" markerHeight="6" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowheadPath" style="stroke-width: 1px; stroke-dasharray: 1px, 0px;"></path></marker></defs></g></g><g class="edgeLabels"><g class="edgeLabel" style="opacity: 1;" transform="translate(170.0749969482422,38.85832977294922)"><g transform="translate(-31.875,-13.358329772949219)" class="label"><rect rx="0" ry="0" width="63.75" height="26.716659545898438"></rect><foreignObject width="63.75" height="26.716659545898438"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span id="L-L-A-B" class="edgeLabel L-LS-A' L-LE-B">Link text</span></div></foreignObject></g></g><g class="edgeLabel" style="opacity: 1;" transform=""><g transform="translate(0,0)" class="label"><rect rx="0" ry="0" width="0" height="0"></rect><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span id="L-L-A-C" class="edgeLabel L-LS-A' L-LE-C"></span></div></foreignObject></g></g><g class="edgeLabel" style="opacity: 1;" transform=""><g transform="translate(0,0)" class="label"><rect rx="0" ry="0" width="0" height="0"></rect><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span id="L-L-B-D" class="edgeLabel L-LS-B' L-LE-D"></span></div></foreignObject></g></g><g class="edgeLabel" style="opacity: 1;" transform=""><g transform="translate(0,0)" class="label"><rect rx="0" ry="0" width="0" height="0"></rect><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;"><span id="L-L-C-D" class="edgeLabel L-LS-C' L-LE-D"></span></div></foreignObject></g></g></g><g class="nodes"><g class="node default" style="opacity: 1;" id="flowchart-A-72" transform="translate(60.599998474121094,90.96665954589844)"><rect rx="0" ry="0" x="-52.599998474121094" y="-23.35832977294922" width="105.19999694824219" height="46.71665954589844" class="label-container"></rect><g class="label" transform="translate(0,0)"><g transform="translate(-42.599998474121094,-13.358329772949219)"><foreignObject width="85.19999694824219" height="26.716659545898438"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;">Square Rect</div></foreignObject></g></g></g><g class="node default" style="opacity: 1;" id="flowchart-B-73" transform="translate(277.0249938964844,38.85832977294922)"><circle x="-30.85832977294922" y="-23.35832977294922" r="30.85832977294922" class="label-container"></circle><g class="label" transform="translate(0,0)"><g transform="translate(-20.85832977294922,-13.358329772949219)"><foreignObject width="41.71665954589844" height="26.716659545898438"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;">Circle</div></foreignObject></g></g></g><g class="node default" style="opacity: 1;" id="flowchart-C-75" transform="translate(277.0249938964844,143.07498931884766)"><rect rx="5" ry="5" x="-50.07499694824219" y="-23.35832977294922" width="100.14999389648438" height="46.71665954589844" class="label-container"></rect><g class="label" transform="translate(0,0)"><g transform="translate(-40.07499694824219,-13.358329772949219)"><foreignObject width="80.14999389648438" height="26.716659545898438"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;">Round Rect</div></foreignObject></g></g></g><g class="node default" style="opacity: 1;" id="flowchart-D-77" transform="translate(435.9599838256836,90.96665954589844)"><polygon points="58.85999450683594,0 117.71998901367188,-58.85999450683594 58.85999450683594,-117.71998901367188 0,-58.85999450683594" transform="translate(-58.85999450683594,58.85999450683594)" class="label-container"></polygon><g class="label" transform="translate(0,0)"><g transform="translate(-32.041664123535156,-13.358329772949219)"><foreignObject width="64.08332824707031" height="26.716659545898438"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; white-space: nowrap;">Rhombus</div></foreignObject></g></g></g></g></g></g></svg></pre>
<blockquote>
<p>Written with <a href="https://stackedit.io/">StackEdit</a>.</p>
</blockquote>
</div>
</body>

</html>
