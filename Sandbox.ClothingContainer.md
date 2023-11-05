# ClothingContainer

## Derives from object

## Summary

Holds a collection of clothing items. Won't let you add items that aren't compatible.
## Constructors

```c#
ClothingContainer( ) 
```
No Summary
## Fields

```c#
List<Clothing> Clothing
```
No Summary
## Methods

```c#
void ClearEntities( ) 
```
No Summary
```c#
void Deserialize( string json) 
```
Deserialize from Json
```c#
void DressEntity( AnimatedEntity citizen, bool hideInFirstPerson = true, bool castShadowsInFirstPerson = true) 
```
Dress this citizen with clothes defined inside this class. We'll save the created entities in ClothingModels.
All clothing entities are tagged with "clothes".
```c#
List<SceneModel> DressSceneObject( SceneModel citizen) 
```
Dress this citizen with clothes defined inside this class. We'll save the created entities in ClothingModels.
All clothing entities are tagged with "clothes".
```c#
IEnumerable<ValueTuple<string, int>> GetBodyGroups( ) 
```
Return a list of bodygroups and what their value should be
```c#
IEnumerable<ValueTuple<string, int>> GetBodyGroups( IEnumerable<Clothing> items) 
```
Return a list of bodygroups and what their value should be
```c#
bool Has( Clothing clothing) 
```
Returns true if we have this clothing item
```c#
void LoadFromClient( IClient cl) 
```
Load the clothing from this client's data. This is a different entry
point than just calling Deserialize directly because if we have
inventory based skins at some point, we can validate ownership here
```c#
string Serialize( ) 
```
Serialize to Json
```c#
void Toggle( Clothing clothing) 
```
Add a clothing item if we don't already contain it, else remove it
## Nested Types

