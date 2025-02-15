
# Resource

> To start api dev serve, please type in your terminal: "<span style="color: #3daaff">nx serve api</span>"

> #### (***BASE_URL***): "localhost:3333"

> <h3 style="color: #18c2a2; ">You can test request (without POSTMAN) by req.http at: <p style="font-size: 14px; color: #18c2a2; ">apps/api/src/test/req.http - have all example in that file</p></h3>


> Api for ***Items***

| Description | Method | URL | Param| Request Body | Example  (response)|
| ----------- | ------ | --- | ---- | ------------ | ------ |
|Get all items|GET|<span style="color: #56A0DF">**/items**</span>| <span style="color: deeppink">null</span> | <span style="color: deeppink">null</span>| <pre style="color: white;">{ <br/>&nbsp;&nbsp; status: "success", <br/>&nbsp;&nbsp; statusCode: "00",<br/>&nbsp;&nbsp; message: "success",<br/>&nbsp;&nbsp; data: [<br/>&nbsp;&nbsp;&nbsp;&nbsp; {<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_id: 60701a429792962528154d94,<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;name: "The Transporter 3",<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;qty: 200,<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;desc: "Release 2004",<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br/>&nbsp;&nbsp;&nbsp;]<br/>}</pre>                                   
|Get a item follow id|GET|<span style="color: #56A0DF">**/item/{id}**</span>|<span style="color: #56A0DF">**id**</span> | <span style="color: deeppink">null</span>|<pre style="color: white;">{ <br/>&nbsp;&nbsp; status: "success", <br/>&nbsp;&nbsp; statusCode: "00",<br/>&nbsp;&nbsp; message: "success",<br/>&nbsp;&nbsp; data: {<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_id: 60701a429792962528154d94,<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;name: "The Transporter 3",<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;qty: 200,<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;desc: "Release 2004",<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br/>&nbsp;&nbsp;&nbsp;<br/>}</pre>
|Delete a item follow id|DELETE|<span style="color: #56A0DF">**/item/{id}**</span>|<span style="color: #56A0DF">**id**</span> | <span style="color: deeppink">null</span>|<pre style="color: white;">{ <br/>&nbsp;&nbsp; status: "success", <br/>&nbsp;&nbsp; statusCode: "00",<br/>&nbsp;&nbsp; message: "success",<br/>&nbsp;&nbsp; data: deleted<br/>}</pre>
|Update a item follow id|PUT|<span style="color: #56A0DF">**/item/{id}**</span>|<span style="color: #56A0DF">**id**</span> | <pre style="color: white">{ <br>&nbsp;&nbsp;name?: string, <br>&nbsp; desc?: string, <br/>&nbsp;&nbsp;qty?: number <br>}</span>|<pre style="color: white;">{ <br/>&nbsp;&nbsp; status: "success", <br/>&nbsp;&nbsp; statusCode: "00",<br/>&nbsp;&nbsp; message: "success",<br/>&nbsp;&nbsp; data: {<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_id: 60701a429792962528154d94,<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;name: "The Transporter 3",<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;qty: 200,<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;desc: "Release 2004",<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br/>&nbsp;&nbsp;&nbsp;<br/>}</pre>
|Create new item|POST|<span style="color: #56A0DF">**/item**</span>|<span style="color: deeppink">null</span> |  <pre style="color: white">{ <br>&nbsp;&nbsp;name: string, <br>&nbsp; desc: string, <br/>&nbsp;&nbsp;qty: number <br>}</span>|<pre style="color: white;">{ <br/>&nbsp;&nbsp; status: "success", <br/>&nbsp;&nbsp; statusCode: "00",<br/>&nbsp;&nbsp; message: "success",<br/>&nbsp;&nbsp; data: {<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_id: 60701a429792962528154d94,<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;name: "Không Thấy Ngày về",<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;qty: 200,<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;desc: "xa bo vai dai",<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br/>&nbsp;&nbsp;&nbsp;<br/>}</pre>

> Api for ***Product*** 

| Description | Method | URL | Param| Request Body | Example (response)|
| ----------- | ------ | --- | ---- | ------------ | ------- |
|Get all products|GET|<span style="color: #56A0DF">**/items**</span>| <span style="color: deeppink">null</span> | <span style="color: deeppink">null</span>|<pre style="color: white;">{ <br/>&nbsp;&nbsp; status: "success", <br/>&nbsp;&nbsp; statusCode: "00",<br/>&nbsp;&nbsp; message: "success",<br/>&nbsp;&nbsp; data: [<br/>&nbsp;&nbsp;&nbsp;&nbsp; {<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_id: 60701a429792962528154d94,<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;title: "The Transporter 3",<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;description: "Release 2004",<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;price: 200,<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br/>&nbsp;&nbsp;&nbsp;]<br/>}</pre>
|Get a product follow id|GET|<span style="color: #56A0DF">**/item/{id}**</span>|<span style="color: #56A0DF">**id**</span> | <span style="color: deeppink">null</span>|<pre style="color: white;">{ <br/>&nbsp;&nbsp; status: "success", <br/>&nbsp;&nbsp; statusCode: "00",<br/>&nbsp;&nbsp; message: "success",<br/>&nbsp;&nbsp; data: {<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_id: 60701a429792962528154d94,<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;title: "The Transporter 3",<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;description: "Release 2004",<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;price: 200,<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br/>&nbsp;&nbsp;&nbsp;<br/>}</pre>
|Delete a product follow id|DELETE|<span style="color: #56A0DF">**/item/{id}**</span>|<span style="color: #56A0DF">**id**</span> | <span style="color: deeppink">null</span>|<pre style="color: white;">{ <br/>&nbsp;&nbsp; status: "success", <br/>&nbsp;&nbsp; statusCode: "00",<br/>&nbsp;&nbsp; message: "success",<br/>&nbsp;&nbsp; data: deleted<br/>}</pre>
|Update a product follow id|PUT|<span style="color: #56A0DF">**/item/{id}**</span>|<span style="color: #56A0DF">**id**</span> | <pre style="color: white">{ <br>&nbsp;&nbsp;title?: string, <br>&nbsp; description?: string, <br/>&nbsp;&nbsp;price?: number <br>}</span>|<pre style="color: white;">{ <br/>&nbsp;&nbsp; status: "success", <br/>&nbsp;&nbsp; statusCode: "00",<br/>&nbsp;&nbsp; message: "success",<br/>&nbsp;&nbsp; data: {<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_id: 60701a429792962528154d94,<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;title: "The Transporter 3",<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;description: "Release 2004",<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;price: 200,<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br/>&nbsp;&nbsp;&nbsp;<br/>}</pre>
|Create new product|POST|<span style="color: #56A0DF">**/item**</span>|<span style="color: deeppink">null</span> |  <pre style="color: white">{ <br>&nbsp;&nbsp;title: string, <br>&nbsp; description: string, <br/>&nbsp;&nbsp;price: number <br>}</span>|<pre style="color: white;">{ <br/>&nbsp;&nbsp; status: "success", <br/>&nbsp;&nbsp; statusCode: "00",<br/>&nbsp;&nbsp; message: "success",<br/>&nbsp;&nbsp; data: {<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_id: 60701a429792962528154d94,<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;title: "The Transporter 3",<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;description: "Release 2004",<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;price: 200,<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br/>&nbsp;&nbsp;&nbsp;<br/>}</pre>



<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

![](https://github.githubassets.com/images/modules/logos_page/Octocat.png)
