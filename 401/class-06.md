# Read 06

## Review

- Define three related pieces of data in a possible application.
An example for a store application might be Product, Category and Department. Describe the constraints and rules on each piece of data and how you would relate these pieces to each other. For example, each Product has a Category and belongs in a Department.
Student, field, university.
Each student is in a field which belongs in a university, one student can be in separate fields but not in separate universities, fields in a university aren't unique but they are connected to each university separately.

- What is the advantage of an ORM, like Mongoose?
More organized, more productive.

- How does the repository pattern compare with an ORM?
ORM handles objects while Repository pattern doesn't.

- When making a repository/facade, what flexibility do you gain?
You don't have to be limited by the other facades, since it can exist on its own.

- Name 3 cloud based NoSQL Databases
Couchbase.
Amazon DynamoDB.
MongoDB.


## Preparation summary

### HTTP

HTTP stands for Hypertext Transfer Protocol. It's a stateless, application-layer protocol for communicating between distributed systems, and is the foundation of the modern web. As a web developer, we all must have a strong understanding of this protocol.

HTTP allows for communication between a variety of hosts and clients, and supports a mixture of network configurations.

To make this possible, it assumes very little about a particular system, and does not keep state between different message exchanges.

This makes HTTP a stateless protocol. The communication usually takes place over TCP/IP, but any reliable transport can be used. The default port for TCP/IP is 80, but other ports can also be used.

![img](https://cdn.tutsplus.com/net/authors/jeremymcpeak/http1-request-response.png)

### REST


What is REST
REST is acronym for REpresentational State Transfer. It is architectural style for distributed hypermedia systems and was first presented by Roy Fielding in 2000 in his famous dissertation.

Like any other architectural style, REST also does have it’s own 6 guiding constraints which must be satisfied if an interface needs to be referred as RESTful. These principles are listed below.

Guiding Principles of REST
Client–server – By separating the user interface concerns from the data storage concerns, we improve the portability of the user interface across multiple platforms and improve scalability by simplifying the server components.
Stateless – Each request from client to server must contain all of the information necessary to understand the request, and cannot take advantage of any stored context on the server. Session state is therefore kept entirely on the client.
Cacheable – Cache constraints require that the data within a response to a request be implicitly or explicitly labeled as cacheable or non-cacheable. If a response is cacheable, then a client cache is given the right to reuse that response data for later, equivalent requests.
Uniform interface – By applying the software engineering principle of generality to the component interface, the overall system architecture is simplified and the visibility of interactions is improved. In order to obtain a uniform interface, multiple architectural constraints are needed to guide the behavior of components. REST is defined by four interface constraints: identification of resources; manipulation of resources through representations; self-descriptive messages; and, hypermedia as the engine of application state.
Layered system – The layered system style allows an architecture to be composed of hierarchical layers by constraining component behavior such that each component cannot “see” beyond the immediate layer with which they are interacting.
Code on demand (optional) – REST allows client functionality to be extended by downloading and executing code in the form of applets or scripts. This simplifies clients by reducing the number of features required to be pre-implemented.