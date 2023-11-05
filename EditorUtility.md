# EditorUtility

## 
```c#
Derives from object
```

## Summary

Set the object to be inspected by the inspector.
## Properties

```c#
static object InspectorObject { get; set; } 
```
Set the object to be inspected by the inspector.
```c#
static bool IsRecordingVideo { get; } 
```
True if we're currently recording a video (using the video command, or F6)
```c#
static bool IsVulkan { get; } 
```
Used for shadergraph
## Methods

```c#
static void ClearPackageCache( ) 
```
Delete the cached package info. This will cause any future requests to get fresh information
from the backend. This is useful if you just updated something and want to see the changes.
```c#
static void CopyAssetToDirectory( Asset asset, string directory, bool overwrite = true) 
```
Copies an asset's source and compiled files to a directory (if they exist)
```c#
static SceneWorld CreateSceneWorld( ) 
```
No Summary
```c#
static VideoWriter CreateVideoWriter( string path, Config config) 
```
Create a video writer
```c#
static WebSurface CreateWebSurface( ) 
```
Create an unlimited web surface
```c#
static IDisposable DisableTextureStreaming( ) 
```
Force textures to load fully when loading a model etc..
```c#
static Task<bool> DownloadAsync( string url, string targetfile, Callback progress = null, CancellationToken token = null) 
```
No Summary
```c#
static HashSet<IPanel> GetRootPanels( ) 
```
Get all the root panels.
```c#
static SceneCamera[] GetSceneCameras( ) 
```
Return all known SceneCameras. This list might have cameras that are no longer active
but haven't been garbage collected yet.
```c#
static SerializedObject GetSerializedObject( object obj) 
```
Get a serialized object for this object. Because you're in the editor, this is an
unrestricted object, we aren't whitelisting or using TypeLibrary.
```c#
static void MoveAssetToDirectory( Asset asset, string directory, bool overwrite = true) 
```
Moves an asset's source and compiled files to a directory (if they exist)
```c#
static void OpenFileFolder( string filepath) 
```
Open given file's folder in OS file explorer and select given file.
```c#
static void OpenFolder( string path) 
```
Open a folder (or url)
```c#
static bool PlayAssetSound( Asset asset) 
```
No Summary
```c#
static bool PlayRawSound( string file) 
```
Plays a sound via the OS, which is the way you play a sound if you
want it to be heard when the game is tabbed away
```c#
static int PlaySound( string sound, float time = 0) 
```
No Summary
```c#
static Task<bool> PutAsync( Stream fileStream, string endpoint, Callback progress = null, CancellationToken token = null) 
```
No Summary
```c#
static void Quit( ) 
```
Quit the whole engine
```c#
static void RenameAsset( Asset asset, string newName) 
```
Moves a file to the same directory but gives it a new name
```c#
static void SendToRecycleBin( string filename) 
```
No Summary
```c#
static void StopSound( int sound) 
```
No Summary
## Events

```c#
static OnInspect( object obj) 
```
Called when InspectorObject changes
## Nested Types

