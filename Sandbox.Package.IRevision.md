# IRevision

## Is interface

## Summary

When this revision was created.
## Properties

```c#
abstract DateTimeOffset Created { get; } 
```
When this revision was created.
```c#
abstract int EngineVersion { get; } 
```
Engine version of this revision.
TODO: How exactly is this different fromPackage.EngineVersion?
```c#
abstract long FileCount { get; } 
```
Number of files in this revision.
```c#
abstract ManifestSchema Manifest { get; } 
```
Manifest of the revision, describing what files are available. For this to be available
you should call DownloadManifestAsync first.
```c#
abstract long TotalSize { get; } 
```
Total size of all the files in this revision, in bytes.
```c#
abstract long VersionId { get; } 
```
Unique index of this revision.
## Methods

```c#
abstract Task DownloadManifestAsync( CancellationToken token = null) 
```
The manifest will not be immediately available until you've downloaded it.
