# WebSocket

## ```c#
Implements IDisposable
```

## Summary

A WebSocket client for connecting to external services.
## Remarks

## Constructors

```c#
WebSocket( int maxMessageSize = 65536) 
```
Initialized a new WebSocket client.
## Properties

```c#
bool EnableCompression { set; } 
```
Enable or disable compression for the websocket. If the server supports it, compression will be enabled for all messages.
Note: compression is disabled by default, and can be dangerous if you are sending secrets across the network.
```c#
bool IsConnected { get; } 
```
Returns true as long as a WebSocket connection is established.
```c#
string SubProtocol { get; } 
```
Get the sub-protocol that was negotiated during the opening handshake.
## Methods

```c#
virtual void Dispose( ) 
```
ImplementsIDisposable.DisposeCleans up resources used by the WebSocket client. This will also immediately close the connection if it is currently open.
```c#
void AddSubProtocol( string protocol) 
```
Add a sub-protocol to be negotiated during the WebSocket connection handshake.
```c#
Task Connect( string websocketUri, CancellationToken ct = null) 
```
Establishes a connection to an external WebSocket service.
```c#
Task Connect( string websocketUri, Dictionary<string, string> headers, CancellationToken ct = null) 
```
Establishes a connection to an external WebSocket service.
```c#
ValueTask Send( string message) 
```
Sends a text message to the WebSocket server.
```c#
ValueTask Send( byte[] data) 
```
Sends a binary message to the WebSocket server.
```c#
ValueTask Send( ArraySegment<byte> data) 
```
Sends a binary message to the WebSocket server.
```c#
ValueTask Send( Span<byte> data) 
```
Sends a binary message to the WebSocket server.
## Events

```c#
OnDataReceived( Span<byte> data) 
```
Event which fires when a binary message is received from the server.
```c#
OnDisconnected( int status, string reason) 
```
Event which fires when the connection to the WebSocket service is lost, for any reason.
```c#
OnMessageReceived( string message) 
```
Event which fires when a text message is received from the server.
## Nested Types

