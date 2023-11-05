# TypeDescription

## ```c#
Derives from object
```

## Summary

Describes a type. We use this class to wrap and return System.Type's that are safe to interact with.Returned byInternal.TypeLibrary.
## Properties

```c#
string[] Aliases { get; } 
```
Possible aliases for this type or member, if any. (AliasAttribute)
```c#
TypeDescription BaseType { get; } 
```
The base type. This can return null if the type isn't in the type library!
```c#
string ClassName { get; } 
```
A string representing this class name. Historically this was provided by [Library( classname )].
If no special name is provided, this will be type.Name.
```c#
string Description { get; } 
```
The summary or description of this type or member.
```c#
FieldDescription[] Fields { get; } 
```
All fields on this type.
```c#
string FullName { get; } 
```
Full name of this type.
```c#
Type[] GenericArguments { get; } 
```
If we're a generic type this will return our generic parameters.
```c#
string Group { get; } 
```
Group or category of this type or member. (CategoryAttribute)
```c#
string Icon { get; } 
```
Material icon of this type or member. (IconAttribute)
```c#
int Identity { get; } 
```
An integer that represents this type. Based off the class name.
```c#
Type[] Interfaces { get; } 
```
If we implement any interfaces they will be here
```c#
bool IsAbstract { get; } 
```
Gets a value indicating whether the System.Type is abstract and must be overridden.
```c#
bool IsClass { get; } 
```
True if the target type is a class
```c#
bool IsEnum { get; } 
```
True if the target type is an enum
```c#
bool IsGenericType { get; } 
```
True if we're a generic type
```c#
bool IsInterface { get; } 
```
True if the target type is an interface
```c#
bool IsStatic { get; } 
```
True if the target type is static
```c#
bool IsValid { get; } 
```
Whether the class is valid or not, i.e. whether the type still exists.
```c#
bool IsValueType { get; } 
```
True if the target type is a value
```c#
MemberDescription[] Members { get; } 
```
All members (methods, properties, etc) of this type.
```c#
MethodDescription[] Methods { get; } 
```
All methods of this type.
```c#
string Name { get; } 
```
Name of this type.
```c#
string Namespace { get; } 
```
Namespace of this type.
```c#
PropertyDescription[] Properties { get; } 
```
All properties of this type.
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
Tags are set via the [Tag] attribute
```c#
Type TargetType { get; } 
```
The type this class describes.
```c#
string Title { get; } 
```
The name of this type or member.
## Methods

```c#
T Create<T,>( object[] args = null) 
```
Create an instance of this class, return it as a T.
If it can't be cast to a T we won't create it and will return null.
```c#
T CreateGeneric<T,>( Type[] typeArgs = null, object[] args = null) 
```
Create an instance of this class using generic arguments
We're going to assume you know what you're doing here and let it throw any exceptions it wants.
```c#
T GetAttribute<T,>( ) 
```
Returns the first attribute of given type, if any are present.
```c#
T GetAttribute<T,>( bool inherited) 
```
Returns the first attribute of given type, if any are present.
```c#
IEnumerable<T> GetAttributes<T,>( bool inherited) 
```
Returns all attributes of given type, if any are present.
```c#
IEnumerable<T> GetAttributes<T,>( ) 
```
Returns all attributes of given type, if any are present.
```c#
MethodDescription GetMethod( string name) 
```
Get a method by name
```c#
PropertyDescription GetProperty( string name) 
```
Get property by name
```c#
bool HasAttribute<T,>( bool inherited = true) 
```
Returns true if the class has this attribute
```c#
bool HasTag( string tag) 
```
True if we have this tag.
```c#
bool IsNamed( string name) 
```
Returns true if this is named the passed name, either through classname, target class name or an alias
```c#
Type MakeGenericType( Type[] typeArgs) 
```
For generic type definitions, create a type by substituting the given types for each type parameter.
We're going to assume you know what you're doing here and let it throw any exceptions it wants.
```c#
override string ToString( ) 
```
OverridesObject.ToString
