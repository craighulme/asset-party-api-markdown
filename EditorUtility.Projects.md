# Projects

## 
```c#
Derives from object
```

## Summary

Wait for the local compiles to be finished
## Methods

```c#
static Task<CompilerOutput[]> Compile( LocalProject project, Action<string> logOutput) 
```
No Summary
```c#
static Task<LocalProject> DownloadCloudProjectAsync( Package package, string folder, CancellationToken cancelToken, Action<string, float> onProgress = null) 
```
No Summary
```c#
static IReadOnlyList<LocalProject> GetAll( ) 
```
No Summary
```c#
static void Remove( LocalProject addon) 
```
No Summary
```c#
static Task SetActiveGame( LocalProject project, Action<string, float> onProgress, CancellationToken ct) 
```
No Summary
```c#
static LocalProject TryAddFromFile( string addonFilePath) 
```
No Summary
```c#
static void UpdateAssetPaths( ) 
```
No Summary
```c#
static void Updated( LocalProject addon, bool paths) 
```
No Summary
```c#
static void UpgradeSchema( LocalProject addon) 
```
No Summary
```c#
static Task WaitForCompiles( ) 
```
Wait for the local compiles to be finished
## Nested Types

