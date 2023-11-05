# AssetSystem

## Is static
Derives from object

## Summary

The asset system, provides access to all the assets.
## Properties

```c#
static IEnumerable<Asset> All { get; } 
```
All the assets that are being tracked by the asset system. Does not include deleted assets.
## Methods

```c#
static bool CompileResource( string path, string text) 
```
Compile a resource from text.
```c#
static bool CompileResource( string path, ReadOnlySpan<byte> data) 
```
Compile a resource from binary data.
```c#
static Asset CreateResource( string type, string absoluteFilename) 
```
Create an emptySandbox.GameResource.
```c#
static void DeleteOrphans( ) 
```
Delete orphaned trivial children. These are things that are generated for
usage by an asset, but aren't referenced by anything, so are useless.
```c#
static Asset FindByPath( string path) 
```
Find an asset by path.
```c#
static Task<Asset> InstallAsync( string packageIdent, Action<float> loading = null, CancellationToken token = null) 
```
Install a cloud package. Will return the primary asset on completion (if it has one)
```c#
static bool IsCloudInstalled( string packageIdent) 
```
Is this package installed in our cloud directory?
```c#
static Asset RegisterFile( string absoluteFilePath) 
```
If you just created an asset, you probably want to immediately register it
## Nested Types

