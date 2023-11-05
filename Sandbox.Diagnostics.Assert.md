# Assert

## Is static
Derives from object

## Summary

Throws an exception when the 2 given objects are not equal to each other.
## Methods

```c#
static void AreEqual<T,>( T a, T b, string message = null) 
```
Throws an exception when the 2 given objects are not equal to each other.
```c#
static void AreNotEqual<T,>( T a, T b, string message = null) 
```
Throws an exception when the 2 given objects are equal to each other.
```c#
static void False( bool isValid, string message = null) 
```
Throws an exception when given expression does not resolve tofalse.
```c#
static void IsNull<T,>( T obj, string message) 
```
Throws an exception when the given object is not null.
```c#
static void IsNull<T,>( T obj) 
```
Throws an exception when the given object is not null.
```c#
static void IsValid( IValid obj) 
```
Throws an exception when the given object is not valid.
```c#
static void NotNull<T,>( T obj, string message) 
```
Throws an exception when the given object is null.
```c#
static void NotNull<T,>( T obj) 
```
Throws an exception when the given object is null.
```c#
static void True( bool isValid, string message = null) 
```
Throws an exception when given expression does not resolve totrue.
