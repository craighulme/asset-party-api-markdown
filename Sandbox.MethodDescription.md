# MethodDescription

## Derives from MemberDescription

## Summary

Describes a method. We use this class to wrap and return MethodInfo's that are safe to interact with.Returned byInternal.TypeLibraryandSandbox.TypeDescription.
## Properties

```c#
ParameterInfo& Parameters { get; } 
```
Gets a list of parameters expected by this method
```c#
Type ReturnType { get; } 
```
Gets the return type of this method.
```c#
override bool IsMethod { get; } 
```
OverridesMemberDescription.IsMethodReturns true - because this is a method
## Methods

```c#
T CreateDelegate<T,>( ) 
```
Creates a delegate bound to this method.
```c#
T CreateDelegate<T,>( object target) 
```
Creates a delegate bound to this method.
```c#
Delegate CreateDelegate( Type delegateType) 
```
Creates a delegate bound to this method.
```c#
Delegate CreateDelegate( Type delegateType, object target) 
```
Creates a delegate bound to this method.
```c#
void Invoke( object targetObject, object[] parameters = null) 
```
Invokes this method.
```c#
T InvokeWithReturn<T,>( object targetObject, object[] parameters = null) 
```
Invokes this method and returns a value.
