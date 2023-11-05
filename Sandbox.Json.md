# Json

## ```c#
Derives from object
```

## Summary

A convenience JSON helper that handlesSandbox.Resourcetypes for you.
## Methods

```c#
static object Deserialize( string source, Type t) 
```
Try to deserialize given source to given type.
```c#
static T Deserialize<T,>( string source) 
```
Try to deserialize given source to given type.
```c#
static object FromNode( JsonNode node, Type type) 
```
Deserialize a single object to a type
```c#
static string Serialize( object source) 
```
Serialize an object.
```c#
static JsonNode ToNode( object obj) 
```
Serialize a single object to a JsonNode
```c#
static JsonNode WalkJsonTree( JsonNode node, Func<string, JsonValue, JsonNode> onValue) 
```
Deep walk though an entire Json tree, optionally changing values of nodes.
