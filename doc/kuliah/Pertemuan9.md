RADIUS is an acronym for Remote Authentication Dial In User Service. RADIUS defines a popular standard used for maintaining and managing remote user authentication and validation. The new Routing and Remote Access Service (RRAS) can operate as a RADIUS client. This allows RAS clients and dial-up routers to be authenticated against a RADIUS server.

RADIUS is defined by RFC 2138. The following is an excerpt from RFC 2138:
Key features of RADIUS are: 

Client/Server Model 

A Network Access Server (NAS) operates as a client of RADIUS. The client is responsible for passing user information to designated RADIUS servers, and then acting on the response which is returned. 

RADIUS servers are responsible for receiving user connection requests, authenticating the user, and then returning all configuration information necessary for the client to deliver service to the user. 

A RADIUS server can act as a proxy client to other RADIUS servers or other kinds of authentication servers. 

Network Security 

Transactions between the client and RADIUS server are authenticated through the use of a shared secret, which is never sent over the network. In addition, any user passwords are sent encrypted between the client and RADIUS server, to eliminate the possibility that someone snooping on an unsecure network could determine a user's password. 

Flexible Authentication Mechanisms 

The RADIUS server can support a variety of methods to authenticate a user. When it is provided with the user name and original password given by the user, it can support PPP PAP, CHAP, UNIX login, and other authentication mechanisms. 

Extensible Protocol 

All transactions are comprised of variable length Attribute-Length-Value 3-tuples. New attribute values can be added without disturbing existing implementations of the protocol.
