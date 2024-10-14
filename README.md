# Assignment-1-Designing-a-Real-time-Application-with-REST-GraphQL-and-WebSockets

The use of REST, GraphQL and websockets for the real-time chat application and the technology recommendation and justification for the following.
Section 1: REST and GraphQL for Data Requests and Updates
•	REST: REST can be used to create the user identity resources (post), can use URL’s to identify resources and use http methods to specify operations. 
GET can be used to retrieve the data as user request about other users (communication between the client and the srver)
PUT is used to update the information about the user identity 
Delete: it is used to delete the resource from the server with user request, patch is used to update parts of the resource
                  Pro’s with REST: 
•	REST can work with various layers, such as load balancers or proxies, without clients knowing. 
•	A client doesn't need to know whether it's communicating directly with the end server or with an intermediary along the way. 
•	This allows for more modular architecture that can be more easily scaled and maintained, as components can be added, removed, or updated without affecting other parts of the system.

•	GraphQL: GraphQL use Query and mutation for retrieving and modifying data
Query: is used for retrieving data from the server through user request, this is a read-only fetch operation, it’s how user request specific data from the server. 
It's not something that's predefined or created by the GraphQL server, instead, the client defines it when writing the query
Mutation: If you want to modify data, user can use a mutation. It can be used for creating, updating, or deleting data.

Pros with GraphQL: 
•	GraphQL allows the client to define the structure of the response data.
•	This flexibility eliminates the over-fetching and under-fetching issues found
in REST.



Section 2: WebSockets for Real-time Communication
•	WebSockets: this is not a request response system like GraphQL and REST this allow users to open communication with the server having low latency by reducing 
the overhead of establishing new connections. The initial phase where the client and server agree to switch from an HTTP protocol to a WebSocket protocol. 
This connection is then full duplex, meaning both the client and the server can send and receive messages independently of one another. This makes WebSockets ideal 
for applications requiring live updates, such as chat applications, live feeds, or gaming.

Difference from REST and GraphQL: REST and GraphQL handle discrete, on-demand requests but do not maintain long term connection for continuous data flow. WebSockets
push data in real time, making them ideal for a chat application, where latency and message delivery speed are must.
Section 3: Technology Recommendation and Justification
•	Hybrid Approach:
Using GraphQL with Websockets will be good as it will help to maintain long term connections between user and server. GraphQl will be used to reterive the data such
as history and user information by defining the structure of Query, Websockets will be used for low latency and full duplex communication. 
Justification:
WebSockets are for open ended by directional communication with the handshake the http protocol is converted into websocket protocol, after that 
there is no need to re-establish the connection for each message exchange. Making the chat application run smoother.

CHAT gpt is used for creating the layout of the system 
BRIGHTSPACE is used for accessing and reading the content information.
