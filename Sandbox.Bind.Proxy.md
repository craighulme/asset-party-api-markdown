# Proxy

## ```c#
Derives from object
```

## Summary

Gets and Sets a value from somewhere.
## Constructors

```c#
protected Proxy( ) 
```
No Summary
## Properties

```c#
abstract bool CanRead { get; } 
```
True if we can get the value.
```c#
abstract bool CanWrite { get; } 
```
True if we can set the value
```c#
virtual bool IsValid { get; } 
```
Should returnfalseif the proxy is now invalid, like if the source object was destroyed.
```c#
abstract object Value { get; set; } 
```
Get or set the value.
```c#
string Name { get; protected set; } 
```
Debug name for this property
```c#
WeakReference<object> Target { get; set; } 
```
The object to read data from and write data to.
## Methods

```c#
override string ToString( ) 
```
OverridesObject.ToString
