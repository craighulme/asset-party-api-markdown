# AnimationGraph

## Derives from Resource

## Summary

Whether the animation graph is invalid, or has not yet loaded.
## Properties

```c#
bool IsError { get; } 
```
Whether the animation graph is invalid, or has not yet loaded.
```c#
string Name { get; } 
```
Animation graph file name.
```c#
int ParamCount { get; } 
```
Number of parameters in this animgraph
## Methods

```c#
static AnimationGraph Load( string filename) 
```
Load an animation graph from given file.
```c#
AnimParam<T> GetParameter<T,>( string name) 
```
Get parameter at given name
```c#
AnimParam<T> GetParameter<T,>( int index) 
```
Get parameter at given index
```c#
string GetParameterName( int index) 
```
Get name of parameter at given index
```c#
Type GetParameterType( int index) 
```
Get value type of parameter at given index
```c#
override string ToString( ) 
```
OverridesObject.ToString
