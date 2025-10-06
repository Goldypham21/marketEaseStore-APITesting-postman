<h1>🛒 MarketEase Store API Testing (Postman Project)</h1>

<h2>📘 Overview</h2>
<p>
This project focuses on <strong>API testing</strong> for the <strong>MarketEase Store API</strong>, 
which simulates a grocery store system allowing customers to browse products, manage carts, and place orders.<br>
All tests were executed using <strong>Postman</strong> and organized into a Postman collection for better structure and reusability.
</p>

<h2>🌐 Base URL</h2>
<pre><code>https://simple-grocery-store-api.click</code></pre>

<h2>📌 API Modules Tested</h2>
<p>
The project includes <strong>manual test cases</strong> and <strong>Postman requests</strong> covering the following main modules:
</p>

<h3>1. Status</h3>
<ul>
  <li><code>GET /status</code> – Verify that the API is up and running.</li>
</ul>

<h3>2. Products</h3>
<ul>
  <li><code>GET /products</code> – Retrieve all products.</li>
  <li><code>GET /products/:productId</code> – Retrieve product details by ID.</li>
</ul>

<h3>3. Cart</h3>
<ul>
  <li><code>GET /carts/:cartId</code> – View a cart.</li>
  <li><code>GET /carts/:cartId/items</code> – Retrieve all items in a cart.</li>
  <li><code>POST /carts</code> – Create a new cart.</li>
  <li><code>POST /carts/:cartId/items</code> – Add an item to a cart.</li>
  <li><code>PATCH /carts/:cartId/items/:itemId</code> – Modify the quantity of an item.</li>
  <li><code>PUT /carts/:cartId/items/:itemId</code> – Replace an item in a cart.</li>
  <li><code>DELETE /carts/:cartId/items/:itemId</code> – Remove an item from a cart.</li>
</ul>

<h3>4. Orders</h3>
<ul>
  <li><code>GET /orders</code> – Retrieve all orders (requires authentication).</li>
  <li><code>GET /orders/:orderId</code> – Retrieve a specific order.</li>
  <li><code>POST /orders</code> – Create a new order.</li>
  <li><code>PATCH /orders/:orderId</code> – Update order details.</li>
  <li><code>DELETE /orders/:orderId</code> – Delete an order.</li>
</ul>

<h3>5. Authentication</h3>
<ul>
  <li><code>POST /api-clients</code> – Register a new API client and receive an access token.</li>
</ul>

<h2>🚀 How to Run Tests in Postman</h2>
<ol>
  <li>Import the file: <strong>MarketEase Store API.postman_collection.json</strong></li>
  <li>Set the Base URL to: 
    <pre><code>https://simple-grocery-store-api.click</code></pre>
  </li>
  <li>Execute each folder in sequence: <em>Status → Products → Cart → Authentication → Orders </em></li>
  <li>Check the console or response body for results.</li>
</ol>

<hr>
