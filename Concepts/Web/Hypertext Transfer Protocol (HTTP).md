#concepts #http #web #terminology 

What is HTTP?
?
Hypertext Transfer Protocol (HTTP) is a standardized protocol that defines how information is transmitted and exchanged on the World Wide Web. It serves as the foundation for data communication on the internet, enabling the transfer of various types of data such as text, images, and multimedia. HTTP operates as a request-response protocol, where clients (such as web browsers) send requests to servers to retrieve or send information.

What is HTTP GET?
?
Retrieve information from a server. It is a simple and stateless request where the client sends a request to the server to retrieve a specified resource, typically indicated by a URL. It is idempotent as multiple identical requests return the same result.
   
What is HTTP PUT?
?
This updates or creates a resource. It involves sending data to the server to replace or create the resource at the specified URL. It is expected to be idempotent as it will keep updating the same resource.
   
What is HTTP POST?
?
Clients submit data to be processed to a specified resource on the server. It is commonly used for creating new resources or submitting information, such as form data, to be processed by the server. It is not expected to be idempotent as new resources could be created on each POST.
   
What is HTTP DELETE?
?
Request the removal of a resource identified by a specific URI (Uniform Resource Identifier) on the server. It is a way to instruct the server to delete the resource associated with the provided URL. It is expected to be idempotent.
   
What is HTTP PATCH?
?
Apply partial modifications to a resource on the server. Instead of replacing the entire resource, a PATCH request typically includes only the changes to be applied, making it a more efficient method for updating resources.
   
What is HTTP HEAD?
?   
Request only the headers of a resource, without requesting the actual content. It is often used to retrieve metadata, such as information about the last modification time or content type, without downloading the full resource.
   
What is HTTP CONNECT?
?   
Establish a tunnel to the server identified by a given URI, typically for the purpose of secure communication through proxies. It is commonly associated with the establishment of SSL/TLS connections, allowing clients to connect to servers securely via an intermediary proxy.
   
What is HTTP OPTIONS?
?  
Inquire about the communication options available for a particular resource on the server. It is often used to retrieve information about the allowed methods, supported authentication methods, or other capabilities of a server without actually requesting the resource's content.
   
What is HTTP TRACE?
?   
Typically used for diagnostic purposes. When a client sends a TRACE request to a server, the server echoes back (loop-back) the received request, allowing the client to see how the request is modified as it travels through various proxies or intermediaries. TRACE is not often used in regular application scenarios but can be helpful in debugging and understanding the path of an HTTP request.

![[HTTP Request Methods.gif]]

   
---

Subscribe to our weekly newsletter to get a Free System Design PDF (158 pages): [https://bit.ly/3KCnWXq](https://bit.ly/3KCnWXq)  
   
[#systemdesign](https://www.linkedin.com/feed/hashtag/?keywords=systemdesign&highlightedUpdateUrns=urn%3Ali%3Aactivity%3A7147838111039836160) [#coding](https://www.linkedin.com/feed/hashtag/?keywords=coding&highlightedUpdateUrns=urn%3Ali%3Aactivity%3A7147838111039836160) [#interviewtips](https://www.linkedin.com/feed/hashtag/?keywords=interviewtips&highlightedUpdateUrns=urn%3Ali%3Aactivity%3A7147838111039836160)