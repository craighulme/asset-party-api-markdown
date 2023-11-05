# PublishSettings

## Derives from object

## Summary

This is data that is saved in an asset's meta file under "publish" to configure
its project for uploading.
## Constructors

```c#
PublishSettings( ) 
```
No Summary
## Properties

```c#
bool Allowed { get; } 
```
Is this asset type allowed to be published?
```c#
bool Enabled { get; set; } 
```
Whether the asset should be published or not.
```c#
ProjectConfig ProjectConfig { get; set; } 
```
Project configuration information
## Methods

```c#
LocalProject CreateTemporaryProject( ) 
```
Create a LocalProject usually with the intention of editing and publishing a single asset.
The project isn't stored or listed anywhere, so is considered a transient that you can load
up, edit, save and then throw away.
```c#
void Save( ) 
```
No Summary
