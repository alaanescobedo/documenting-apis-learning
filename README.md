#### **This repository is based on the guide: [API Documentation: A Guide for Technical Writers and Engineers](https://idratherbewriting.com/learnapidoc/).**
------------

## **Categorize API's**
One way to sort the different types of APIs is to categorize them into two general buckets:
- Web service APIs
- Native library APIs

#### More: 
  - SOAP APIs
  - RPC-based APIs
  - gRPC APIs
  - REST APIs
  - GraphQL APIs
  - Voice Assistant APIs
  - Internet of Things (IoT) APIs

### 🔵 **- Native library APIs** (*also called library-based APIs*)
- Refer to code libraries (*for example, JAR files*).
- Involve incorporating code that developers add directly to their projects for the desired functionality.
- Provide additional functionality through classes or other functions that can be called locally. 
- Are language-specific. (*e.g., Java, C++, Python, etc.*).

### 🔵 **- Web service APIs**
- These APIs are typically exposed as RESTful web services.
- Send and receive messages across the web using HTTP to transport the request and response.
- Are language agnostic.

#### → **- Soap APIs** (*Simple Object Access Protocol*)
- Are web services that rely on a strict XML protocol to define the message exchange format for requests and responses. 
- Is common with financial APIs and regulated industries, though it has largely been replaced by REST in popularity.
- As a standardized protocol, SOAP’s XML message format is usually defined through a WSDL (Web Services Description Language) file that specifies the allowed elements and attributes in the message exchange. 
  - The WSDL file is machine-readable and used by the servers interacting with each other to facilitate the communication. 

#### → **- RPC-based APIs** (*Remote Procedure Call*)
- Are web services that call a method on a remote server by delivering an encoded message through HTTP. 
- The encoded message format might be:
  - XML for [XML-RPC APIs](https://en.wikipedia.org/wiki/XML-RPC)
  - JSON for [JSON-RPC APIs](https://en.wikipedia.org/wiki/JSON-RPC)
- In both cases, the message travels to the remote server via **HTTP** like other web services.
- The methods on the remote servers can be in any language.
  - Example: An XML-RPC API can call a Java or Python or C++ method.

#### → **- gRPC APIs** (*Google RPC*)
-  Are web services similar to RPC-based APIs.
    - Calls a function or runs a procedure on a remote server.
- Uses **protocol buffers** (specified in `.proto` files) rather than XML or JSON as the message exchange format.
  - Protocol buffer lets you define the structure for your data and the way to convert (*serialize*) the data to be consumed by the receiving server.
  - Protocol buffers are lighter and more efficient than XML. 
- gRPC APIs were developed by Google and published as an open-source platform.
- More info about [gRPC Apis](https://grpc.io/docs/).

#### → **- REST APIs** (*Representational State Transfer*)
- Are web services that let you make requests for resources through URL paths. 
  - `GET /users/1` - `POST /users`
- The `requests` and `responses` travel via **HTTP** across the web, and the servers receiving the requests are language agnostic about the request (not required to be a specific programming language).
- Responses are typically returned in JSON or XML formats.
- They have different paths (endpoints) with various parameters you can configure to determine the results you want.
- More info about [REST APIs](https://idratherbewriting.com/learnapidoc/docapis_what_is_a_rest_api.html).

#### → **- GraphQL APIs** (*Graph Query Language*)
- Are web services developed by Facebook.
- It allows users dynamically query for the results they need through a single path (endpoint).
- Eliminates the need for multiple request URLs or other post-filtering on the returned results to get what you need.
- Your query retrieves only the needed data, allowing the request and response to be fast and specific.
- More info about [GraphQL APIs](https://graphql.org/).

#### → **- Voice Assistant APIs**
- Are used with voice assistants such as Alexa.
- These APIs originate from the cloud and call an endpoint based on natural language processing of voice commands spoken by users.
- This is a case where APIs operate behind the scenes in the cloud, and developers create code, such as in a `Lambda function` (*cloud computing*), that handles incoming requests sent from the voice assistant API.

#### → **- IoT API's** (*Internet of Things*)
- Are used by physical devices (such as sensors or wearables) that transmit or receive data to connect the device to an online network.

More info about [types of APIs:](https://ffeathers.wordpress.com/2014/02/16/api-types/)
--------------
--------------
