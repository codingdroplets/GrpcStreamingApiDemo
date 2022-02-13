# gRPC Streaming API in .Net C#

Watch Tutorial Video: https://www.youtube.com/watch?v=Vwr9GRD-5is

This is a complete course to develop .Net applications or services with gRPC. This video is part of a series and this is the second video of the gRPC C# Tutorial Series. In this video we cover the types on gRPC Streaming APIs and how to implement those in C# project.

gRPC C# Tutorial Playlist link:
https://www.youtube.com/playlist?list=PLzewa6pjbr3IOa6POjAMM0xiPZ-shjoem

gRPC Streaming APIs are the APIs with which we can stream data. Streaming data means we can send multiple or infinite data without any limitations using a single TCP connection. Streaming data is a highlighted benefit of gRPC APIs, as you know this option is not there in REST APIs. gRPC Streaming APIs are one of the best options if you are dealing with big data. There are three types of grpc streaming APIs.

1. gRPC Server Streaming [Server Streaming RPC]
A server-streaming RPC is like a unary RPC, except that the server returns a stream of messages in response to a client’s request. So, the client can send a single request to the server and the server will responds back with multiple multiple or a stream of messages.

2. gRPC Client Streaming [Client Streaming RPC]
In a client-streaming RPC, the client will send multiple messages or a stream of messages to the server. But the server will respond back with a single message.

3. gRPC Bidirectional Streaming [Bidirectional Streaming RPC]
In Bidirectional streaming RPC both client and server can send multiple messages. That means both request and response will be a stream of messages. Hence Bidirectional Streaming RPC is a two streaming API [C# gRPC two way Stream / DotNet gRPC two way Streaming].

Client- and server-side stream processing is application specific. Since the two streams are independent, the client and server can read and write messages in any order. For example, a server can wait until it has received all of a client’s messages before writing its messages, or the server and client can play “ping-pong” – the server gets a request, then sends back a response, then the client sends another request based on the response, and so on.

gRPC Channel:
A gRPC channel provides a connection to a gRPC server on a specified host and port. It is used when creating a client stub. Clients can specify channel arguments to modify gRPC’s default behavior, such as switching message compression on or off. A channel has state, including connected and idle.
