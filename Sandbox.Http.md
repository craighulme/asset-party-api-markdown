# Http

## 
```c#
Derives from object
```

## Summary

Lets your game make async HTTP requests.
## Methods

```c#
static HttpContent CreateJsonContent<T,>( T target) 
```
Creates a new System.Net.Http.HttpContent instance containing the specified object serialized to JSON.
```c#
static bool IsAllowed( Uri uri) 
```
Check if the given Uri matches the following requirements:Scheme is https/http or wss/wsIf it's localhost, only allow ports 80/443/8080/8443Not an ip address
```c#
static bool IsHeaderAllowed( string header) 
```
Checks if a given header is allowed to be set.
```c#
static Task<HttpResponseMessage> RequestAsync( string requestUri, string method = "GET", HttpContent content = null, Dictionary<string, string> headers = null, CancellationToken cancellationToken = null) 
```
Sends a HTTP request to the specified URI and returns the response in an asynchronous operation.
```c#
static Task<byte[]> RequestBytesAsync( string requestUri, string method = "GET", HttpContent content = null, Dictionary<string, string> headers = null, CancellationToken cancellationToken = null) 
```
Send a HTTP request to the specified URI and return the response body as a byte array in an asynchronous operation.
```c#
static Task<T> RequestJsonAsync<T,>( string requestUri, string method = "GET", HttpContent content = null, Dictionary<string, string> headers = null, CancellationToken cancellationToken = null) 
```
Sends a HTTP request to the specified URI and return the response body as a JSON deserialized object in an asynchronous operation.
```c#
static Task<Stream> RequestStreamAsync( string requestUri, string method = "GET", HttpContent content = null, Dictionary<string, string> headers = null, CancellationToken cancellationToken = null) 
```
Send a HTTP request to the specified URI and return the response body as a stream in an asynchronous operation.
```c#
static Task<string> RequestStringAsync( string requestUri, string method = "GET", HttpContent content = null, Dictionary<string, string> headers = null, CancellationToken cancellationToken = null) 
```
Send a HTTP request to the specified URI and return the response body as a string in an asynchronous operation.
