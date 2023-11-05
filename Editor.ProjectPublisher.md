# ProjectPublisher

## 
```c#
Derives from object
```

## Summary

Get access to the files within the manifest
## Properties

```c#
IEnumerable<ProjectFile> Files { get; } 
```
Get access to the files within the manifest
```c#
AddonManifest Manifest { get; protected set; } 
```
No Summary
```c#
int MissingFileCount { get; } 
```
No Summary
```c#
long MissingFileSize { get; } 
```
No Summary
```c#
Action OnProgressChanged { get; set; } 
```
No Summary
```c#
string TargetPackageIdent { get; } 
```
No Summary
```c#
int TotalFileCount { get; } 
```
No Summary
## Methods

```c#
static bool CanPublishFile( Asset a) 
```
Return true if we're not opposed to publishing this asset
```c#
static Task<ProjectPublisher> FromAsset( Asset asset) 
```
No Summary
```c#
static Task<ProjectPublisher> FromProject( LocalProject project) 
```
No Summary
```c#
Task AddCodePackageReference( string package) 
```
If the code is referencing a package - we can add it to the manifest using this.
```c#
Task AddFile( byte[] contents, string relativePath) 
```
Manually add a file to the manifest
```c#
Task AddFile( string contents, string relativePath) 
```
Manually add a file to the manifest
```c#
Task PrePublish( CancellationToken cancellationToken = null) 
```
Check the intended manifest, ask the backend which files need to be uploaded.
```c#
Task Publish( IProgress progress = null, CancellationToken cancel = null) 
```
Publish a new revision
```c#
void SetChangeDetails( string change, string detail) 
```
Allows to set information on the revision - for future reference
```c#
void SetMeta( string key, object obj) 
```
No Summary
```c#
Task UploadFiles( ) 
```
No Summary
## Nested Types

