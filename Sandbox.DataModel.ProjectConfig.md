# ProjectConfig

## 
```c#
Derives from object
```

## Summary

Configuration of aSandbox.LocalProject.
## Constructors

```c#
ProjectConfig( ) 
```
No Summary
## Properties

```c#
string AssetsPath { get; set; } 
```
A relative path to the assets folder in your addon. HasAssets should be set to true.
Leave this empty to use the root folder as the root of your addon path.
```c#
string CodePath { get; set; } 
```
A relative path to the code for your addon. HasCode should be set to true.
Leave this empty if you want the root folder to host your code.
```c#
DirectoryInfo Directory { get; set; } 
```
The directory housing this addon (TODO)
```c#
List<string> EditorReferences { get; set; } 
```
A list of packages that this package uses but there is no need to install. For example, a map package might use
a model package - but there is no need to download that model package because any usage will organically be included
in the manifest. However, when loading this item in the editor, it'd make sense to install these 'cloud' packages.
```c#
string FullIdent { get; } 
```
Returns a combination of Org and Ident - for example "facepunch.sandbox" or "valve.cs".
```c#
bool HasAssets { get; set; } 
```
If this addon contains models, textures, sounds etc, this should be set to true.
```c#
bool HasCode { get; set; } 
```
If this addon contains code, this should be set to true
```c#
string Ident { get; set; } 
```
The ident of this addon. For example "sandbox", "cs" or "dm98"
```c#
string MenuResources { get; set; } 
```
A list of paths in which to look for extra assets to upload with the addon when used as a menu (games only)
```c#
Dictionary<string, object> Metadata { get; set; } 
```
Custom key-value storage for this project.
```c#
string Org { get; set; } 
```
The ident of the org that owns this addon. For example "facepunch", "valve".
```c#
List<string> PackageReferences { get; set; } 
```
A list of packages that this package depends on. These should be installed alongside this package.
```c#
Type PackageType { get; } 
```
Type of the package.
```c#
string Resources { get; set; } 
```
A list of paths in which to look for extra assets to upload with the addon. Note that compiled asset files are automatically included.
```c#
int Schema { get; set; } 
```
The version of the addon file. Allows us to upgrade internally.
```c#
string Tags { get; set; } 
```
A space separated list of tags
```c#
string Title { get; set; } 
```
The human readable title, for example "Sandbox", "Counter-Strike"
```c#
string Type { get; set; } 
```
The type of addon. Current valid values are "game"
## Methods

```c#
T GetMetaOrDefault<T,>( string keyname, T defaultValue) 
```
Get the package's meta value. If it's missing or the wrong type then use the default value.
```c#
bool SetMeta( string keyname, object outvalue) 
```
Store custom data at given key in theProjectConfig.Metadata.
```c#
string ToJson( ) 
```
Serialize the entire config to a JSON string.
```c#
bool TryGetMeta<T,>( string keyname, out T outvalue) 
```
Try to get a value at given key inProjectConfig.Metadata.
```c#
override string ToString( ) 
```
OverridesObject.ToString
