## How the Internet works

- URL maped with IP address
- DNS Server - takes the url as input and throws ip address as output
- http://cs.harvard.edu/subject/computer-science
- http is a protocol
- .edu is TLD
- hravard is second level domain
- subject/computer science is the resource/file

## Client-Server Architecture

- any end-system that inititaites request is client.
- any end system that recives a request, process the data and send the response is server
- TCP hand shake between client server 
- over the TCP connection there is http request and http response
- Vertical scaling - increment the power of one machine
- horizontal scaling - boot up the multiple machine instead of power of one machine
- load balancer
- Auto Scaling
- Monolithic vs microservices
- client - middle end - backend
- web socket based on tcp, it's not based on request and response based architecture
- it' based on stream and pipe line based architecture
- pm2

## API

- Aplication Programing Interface
- interface means contract so it is contract of application programming
- How to use a application, for that a contract is made that is api
- like web APIs: getelementbyid, settimeout it can also be called function, make a contract by liabrary function call
- what input it takes, what output it will return and what process it will do
- we also communicate over network call by http
- API enable us to provide a way for other people so that they can communicate with our appplication or functionality
- this functionality might be exposed by liabrary call or over network call by http
- API is a contract of how to use some functionality or application, this functionality can be exposed in the internt which is called by http network call or by other liabrary

## Framework vs liabrary

liabary - some specifics functionality provide 
framework - multile liabary combine in frame work

## REST

 - Representational state transfer
 - For any type of communication, there are alwys a set of rules definced and also some recomedation or guidelines
 - REST is a set of guidelines that drive architecture of the web
 - REST API - Any APi that follows the REST guidelines is REST API

 ### other ALternative of REST
 - SOAP
 - GraphQL
 - GRPC
 
### REST Guidelines

- Rset prefer client server communication should happen over http
- Rest prefer JSON as the format to send & recive data
- Rest gives guidelineon how the url should look like
	- in REST the main source of info is consider as resource eg. 
	- tweet -  resource
	- user - resource
	- crate tweet - action
	- delete tweet - action
	- add user - action
	- resource - nouns
	- actions - verbs
	- url focus around resources (noun)	
- the endpoints/url should use Noun & not verbs
	- e,g - medium.com/blogs
	- medium.com/blogs/2
- the noun that be mentioned expected to be plural
- every REST endpoint should be defined along with a http methods
	- GET - retrive data
	- post - send data, create a new resource
	- delete - delete data
	- put - update a resource
	- patch - parallel update resource
	- get/blogs/:id - :id is variable
- we use nesting for relationship
	- eg. blogs/13/comments
	- blogs/22/comments/3
	- don't use more than 3 level nesting
- REST expects the response to have http codes
- API Versioning-  version represent that a relise of  new set of functionality for API
- Sending data can be done in three ways
	- Request body like get ,post (configure using programetically or tools like postman)
	- URL parrams like blogs/22/comments/3
	- query params like /products?category = electronics & company = apple
- framework like rails, django follows REST
- liabrary like axios follows REST
- CRUD API 
