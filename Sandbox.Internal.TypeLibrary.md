# TypeLibrary

## ```c#
Derives from object
```

## Summary

Check if all properties of this class instance pass their System.ComponentModel.DataAnnotations.ValidationAttribute.
## Methods

```c#
bool CheckValidationAttributes<T,>( T obj) 
```
Check if all properties of this class instance pass their System.ComponentModel.DataAnnotations.ValidationAttribute.
```c#
object Create( string name, Type targetType, object[] args = null) 
```
Create a type instance by name and is assignable to given type, with optional arguments for its constructor.
```c#
T Create<T,>( Type type, object[] args = null) 
```
Create type instance from type.
```c#
T Create<T,>( string name = null, bool complainOnMissing = true) 
```
Create a type instance by name and is assignable to given type.
```c#
T Create<T,>( int ident) 
```
Create a type instance by its identity. See Sandbox.Internal.TypeLibrary.GetIdent(System.Type).
```c#
IEnumerable<MethodDescription> FindStaticMethods( string methodName) 
```
Find all static methods with given name.
```c#
IEnumerable<MethodDescription> FindStaticMethods<T,>( string methodName) 
```
Find all static methods with given name and given attribute.
```c#
IEnumerable<MethodDescription> FindStaticMethods<T,>( ) 
```
No Summary
```c#
T GetAttribute<T,>( Type t) 
```
Get single attribute of type, from type
```c#
IEnumerable<T> GetAttributes<T,>( ) 
```
Get all attributes of this type
```c#
IEnumerable<T> GetAttributes<T,>( Type t) 
```
Get all attribute of type, from all types assignable to type
```c#
EnumDescription GetEnumDescription( Type enumType) 
```
Get a class describing the values of an enum
```c#
Type[] GetGenericArguments( Type genericType) 
```
Performs System.Type.GetGenericArguments with access control checks.
Will throw if any arguments aren't in the whitelist.
```c#
IEnumerable<T> GetMemberAttributes<T,>( ) 
```
Find all member attributes (instances) with given attribute type.
```c#
IEnumerable<T> GetMemberAttributes<T,>( bool staticMembers) 
```
Find all static or non static only member attributes (instances) with given attribute type.
```c#
IEnumerable<ValueTuple<MethodDescription, T>> GetMethodsWithAttribute<T,>( ) 
```
Find all static methods with given attribute.
```c#
PropertyDescription[] GetPropertyDescriptions( object obj, bool onlyOwn = false) 
```
Get a list of properties on the target object. To do this we'll just call GetDescription( obj.GetType() ) and return .Properties.
Will return an empty array if we can't access these properties.
```c#
object GetPropertyValue( object target, string name) 
```
Try to get a value from a property on an object
```c#
SerializedObject GetSerializedObject( object target) 
```
Get a SerializedObject version of this object
```c#
TypeDescription GetType( Type type) 
```
Get the description for a specific type. This will return null if you don't have whitelist access to the type.
For constructed generic types, this will give you the description of the generic type definition.
```c#
TypeDescription GetType<T,>( ) 
```
ImplementsObject.GetTypeFind the description for templated type
```c#
TypeDescription GetType( string name) 
```
Find a TypeDescription by name
```c#
TypeDescription GetType<T,>( string name) 
```
Find a TypeDescription that derives from T, by name
```c#
TypeDescription GetTypeByIdent( int ident) 
```
Find a TypeDescription by name
```c#
int GetTypeIdent( Type type) 
```
Get hash of a type.
```c#
IEnumerable<TypeDescription> GetTypes( Type type) 
```
Get descriptions for all types that derive from T
```c#
IEnumerable<TypeDescription> GetTypes<T,>( ) 
```
Get descriptions for all types that derive from T
```c#
IEnumerable<TypeDescription> GetTypes( ) 
```
Get all types
```c#
IEnumerable<ValueTuple<TypeDescription, T>> GetTypesWithAttribute<T,>( ) 
```
Get all attributes of this type. Returns the type description along with the attribute. This will
also return types that inherit the attribute from base classes too.
```c#
IEnumerable<ValueTuple<TypeDescription, T>> GetTypesWithAttribute<T,>( bool inherited) 
```
Get all attributes of this type. Returns the type description along with the attribute.
If inherited is false, we will return only classes that contain this attribute directly.
```c#
bool HasAttribute<T,>( Type type) 
```
Return true if this type contains this attribute
```c#
bool SetProperty( object target, string name, object value) 
```
Set a named property on given object.
Will perform extra magic for string inputs and try to convert to target property type.
```c#
bool TryGetType( Type t, out TypeDescription typeDescription) 
```
Find the description type
```c#
bool TryGetType<T,>( out TypeDescription typeDescription) 
```
Find the description type
