# Builder

## Derives from ValueType

## Summary

A helper to create binds between two properties (or whatever you want)Example usage: set "BoolValue" from value of "StringValue"BindSystem.Build.Set( this, "BoolValue" ).From( this, "StringValue" );
## Methods

```c#
Link From<T,>( T obj, PropertyInfo target) 
```
No Summary
```c#
Link From<T,>( T obj, string targetName) 
```
No Summary
```c#
Link From<T,>( Func<T> read, Action<T> write) 
```
Read and write the Right hand side via custom callbacks, rather than a specific property.
```c#
Link From<T,>( object sourceObject, Func<T> read, Action<T> write) 
```
No Summary
```c#
Link From<T,V,>( T obj, Expression<Func<T, V>> propertyName) 
```
No Summary
```c#
Link From( Proxy source) 
```
No Summary
```c#
Link FromDictionary<K,V,>( Dictionary<K, V> dict, K key) 
```
No Summary
```c#
Link FromObject( object obj) 
```
No Summary
```c#
Builder ReadOnly( bool makeReadOnly = true) 
```
Makes the bind link one way. The system will not try to write to the target/right hand property. (The one you set via "From" methods)
```c#
Builder Set<T,>( T obj, string targetName, Action onChanged = null) 
```
No Summary
```c#
Builder Set<T,U,>( T obj, Func<U> read, Action<U> write) 
```
Call this function when the Right hand changes. Stop updating when the object dies.
```c#
Builder Set( Proxy binding) 
```
No Summary
## Extensions

```c#
Link FromConsoleVariable( string name) 
```
Bind the Left hand side to the value of the given console variable.
```c#
Link FromConsoleVariableInt( string name) 
```
Bind the Left hand side to the value of the given console variable as an integer.
## Referencing Members

```c#
Builder = GraphicsItem.Bind( string ) 
```
```c#
Builder = QObject.Bind( string, Action ) 
```
```c#
Builder = BindSystem.Build { get; } 
```
```c#
static Link = SandboxToolExtensions.FromConsoleVariable( Builder, string ) 
```
```c#
static Link = SandboxToolExtensions.FromConsoleVariableInt( Builder, string ) 
```
