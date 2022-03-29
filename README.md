#### **This repository is based on the guide: [API Documentation: A Guide for Technical Writers and Engineers](https://idratherbewriting.com/learnapidoc/).**
------------

### **Categorize API's**
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