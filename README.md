Write a blog on Difference between HTTP1.1 vs HTTP2

HTTP stands for hypertext transfer protocol & it is used in client-server communication. By using HTTP user sends the request to the server & the server sends the response to the user. There are several stages of development of HTTP but we will focus mainly on HTTP/1.1 which was created in 1997 & the new one is HTTP/2 which was created in 2015.

HTTP/1.1: For better understanding, let’s assume the situation when you make a request to the server for the geeksforgeeks.html page & server responds to you as a resource geeksforgeeks.html page. before sending the request and the response there is a TCP connection established between client & server. again you make a request to the server for image img.jpg & the server gives a response as an image img.jpg. the connection was not lost here after the first request because we add a keep-alive header which is the part of the request so there is an open connection between the server & client. there is a persistent connection which means several requests & responses are merged in a single connection. These are the drawbacks that lead to the creation of HTTP/2: The first problem is HTTP/1.1 transfer all the requests & responses in the plain text message form. The second one is head of line blocking in which TCP connection is blocked all other requests until the response does not receive. all the information related to the header file is repeated in every request.
Ithe usest works on the textual format.
There is head of line blocking that blocks all the requests behind it until it doesn’t get its all resources.
It uses requests resource Inlining for use getting multiple pages.
It compresses data by itself.



HTTP/2: HTTP/2 was developed over the SPDY protocol. HTTP/2 works on the binary framing layer instead of textual that converts all the messages in binary format. it works on fully multiplexed that is one TCP connection is used for multiple requests. HTTP/2 uses HPACK which is used to split data from header. it compresses the header. The server sends all the other files like CSS & JS without the request of the client using the PUSH frame.
It works on the binary protocol.
It allows multiplexing so one TCP connection is required for multiple requests.
It uses PUSH frame by server that collects all multiple pages 
It uses HPACK for data compression.
  
  
  Write a blog about objects and its internal representation in Javascript
  
Objects in JavaScript, just as in many other programming languages, can be compared to objects in real life. The concept of objects in JavaScript can be understood with real life, tangible objects.

In JavaScript, an object is a standalone entity, with properties and type. Compare it with a cup, for example. A cup is an object, with properties. A cup has a color, a design, weight, a material it is made of, etc. The same way, JavaScript objects can have properties, which define their characteristics.

Objects and properties.
A JavaScript object has properties associated with it. A property of an object can be explained as a variable that is attached to the object. Object properties are basically the same as ordinary JavaScript variables, except for the attachment to objects. The properties of an object define the characteristics of the object. You access the properties of an object with a simple dot-notation:

eg;objectName.propertyName

the objects uses the key value pair

syntax
objectname={key:value}

eg:
const myCar = {
  make: 'Ford',
  model: 'Mustang',
  year: 1969
};

console.log(myCar)

Internal representation of object
![image](https://user-images.githubusercontent.com/107340174/174491689-14c104b9-9d7d-4519-b587-64ae34f4b5e2.png)

INternal representation of object accesing the values
![image](https://user-images.githubusercontent.com/107340174/174491816-d51c02be-21ac-4d9c-84bf-7cb596921735.png)



  
