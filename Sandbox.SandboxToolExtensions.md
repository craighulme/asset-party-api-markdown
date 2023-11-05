# SandboxToolExtensions

## 
```c#
Derives from object
```

## Summary

Bind the Left hand side to the value of the given console variable.
## Methods

```c#
static Link FromConsoleVariable( Builder self, string name) 
```
Bind the Left hand side to the value of the given console variable.
```c#
static Link FromConsoleVariableInt( Builder self, string name) 
```
Bind the Left hand side to the value of the given console variable as an integer.
```c#
static Asset[] GetAssets( LocalProject project) 
```
Get all assets in this project
```c#
static bool RenderToPixmap( SceneCamera camera, Pixmap targetPixmap, bool async = false) 
```
Render this camera to the target widget. Once you do this the target widget becomes "externally painted", so you
won't be able to paint on it anymore with Qt's Paint stuff.
```c#
static bool RenderToVideo( SceneCamera camera, VideoWriter videoWriter, TimeSpan? time = null) 
```
Render this camera to the target widget. Once you do this the target widget becomes "externally painted", so you
won't be able to paint on it anymore with Qt's Paint stuff.
```c#
static Task<bool> RenderToVideoAsync( SceneCamera camera, VideoWriter videoWriter, TimeSpan? time = null) 
```
Render this camera to the target widget. Once you do this the target widget becomes "externally painted", so you
won't be able to paint on it anymore with Qt's Paint stuff.
```c#
static Task SetFavouriteAsync( Package package, bool state) 
```
Mark this package as a favourite
```c#
static Task SetVoteAsync( Package package, bool up) 
```
Add your vote for this package
```c#
static Task<bool> UploadFile( Package package, string absolutePath, string relativePath, Callback progress, CancellationToken token = null) 
```
Mark this package as a favourite
```c#
static Task<bool> UploadFile( Package package, byte[] contents, string relativePath, Callback progress, CancellationToken token = null) 
```
Upload a file used by this package
```c#
static Task<bool> UploadVideo( Asset asset, byte[] contents, bool isThumbVideo, bool hidden = false, string tag = null, Callback progress = null, CancellationToken token = null) 
```
Upload a video for this package
