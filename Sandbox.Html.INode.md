# INode

## ```c#
Is interface
```

## Summary

No Summary
## Properties

```c#
abstract IEnumerable<INode> Children { get; } 
```
No Summary
```c#
abstract string InnerHtml { get; } 
```
No Summary
```c#
abstract bool IsComment { get; } 
```
No Summary
```c#
abstract bool IsElement { get; } 
```
No Summary
```c#
abstract bool IsText { get; } 
```
No Summary
```c#
abstract string Name { get; } 
```
No Summary
```c#
abstract string OuterHtml { get; } 
```
No Summary
## Methods

```c#
abstract string GetAttribute( string name, string def = "") 
```
No Summary
```c#
abstract T GetAttribute<T,>( string name, T def = null) 
```
No Summary
```c#
abstract bool GetAttributeBool( string name, bool def = false) 
```
No Summary
```c#
abstract float GetAttributeFloat( string name, float def = 0) 
```
No Summary
```c#
abstract int GetAttributeInt( string name, int def = 0) 
```
No Summary
