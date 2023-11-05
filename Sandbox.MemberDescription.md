# MemberDescription

## Derives from object

## Summary

Wraps MemberInfo but with caching and sandboxing.Returned byInternal.TypeLibraryandSandbox.TypeDescription.
## Properties

```c#
virtual bool IsField { get; } 
```
True if we're a field
```c#
virtual bool IsMethod { get; } 
```
True if we're a method
```c#
virtual bool IsProperty { get; } 
```
True if we're a property
```c#
string[] Aliases { get; } 
```
Aliases allow this to be found by alternative names.
```c#
Attribute[] Attributes { get; } 
```
Attributes on this member
```c#
string Description { get; } 
```
Description of this type member. This usually provided from the summary XML comment above the definition.
```c#
string Group { get; } 
```
The group - usually provided via the [Group] attribute
```c#
string Icon { get; } 
```
The icon for this, if provided via the [Icon] attribute
```c#
bool IsStatic { get; protected set; } 
```
True if static
```c#
string Name { get; } 
```
Name of this type member.
```c#
int Order { get; } 
```
The display order - usually provided via the [Order] attribute
```c#
string SourceFile { get; } 
```
The file containing this member
```c#
int SourceLine { get; } 
```
The line number of this member
```c#
string[] Tags { get; } 
```
Tags are usually provided via the [Tags] attribute
```c#
string Title { get; } 
```
Display name or title of this type member.
```c#
TypeDescription TypeDescription { get; } 
```
The type that we're a member of
## Methods

```c#
T GetCustomAttribute<T,>( ) 
```
Returns the first of Attributes of the passed in type. Or null.
```c#
DisplayInfo GetDisplayInfo( ) 
```
Access the full DisplayInfo for this type. This is faster than creating the DisplayInfo every time we need it.
```c#
bool HasAttribute<T,>( ) 
```
Whether or not this has at least one of the specified attribute.
```c#
bool HasAttribute( Type t) 
```
Whether or not this has at least one of the specified attribute.
```c#
bool HasTag( string tag) 
```
Returns true if Tags contains this tag
```c#
protected void Init( MemberInfo x) 
```
No Summary
```c#
bool IsNamed( string name) 
```
Utility function to check whether this string matches this type. Will search name and classname.
```c#
override string ToString( ) 
```
OverridesObject.ToString
## Inheriting Types

