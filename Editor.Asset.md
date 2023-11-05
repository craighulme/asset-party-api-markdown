# Asset

## ```c#
Derives from object
```

## Summary

The absolute path as it is on disk (ie .wav not .vsnd)
## Properties

```c#
string AbsolutePath { get; } 
```
The absolute path as it is on disk (ie .wav not .vsnd)
```c#
AssetType AssetType { get; } 
```
The type of this asset.
```c#
bool CanRecompile { get; } 
```
Can this asset be recompiled?
```c#
bool IsCached { get; } 
```
Is this asset loaded?
```c#
bool IsCompiled { get; } 
```
Whether the asset is compiled.
```c#
bool IsCompileFailed { get; } 
```
Whether the asset failed to compile.
```c#
bool IsDeleted { get; } 
```
Whether the asset is deleted or not.
This can happen afterAsset.Deletewas called on it, orAsset.AbsolutePathis empty.
```c#
bool IsTrivalChild { get; } 
```
The asset was generated from another asset compile and has no source asset of its own. For example model break gibs .vmdl, .vtex files for materials, etc.
```c#
DateTime? LastOpened { get; } 
```
When the asset was last opened through the editor.
```c#
MetaData MetaData { get; } 
```
Asset type specific key-value based data storage.
```c#
string Name { get; } 
```
Name of the asset, usually the filename.
```c#
Package Package { get; } 
```
If this asset was downloaded from asset.party then this will
be the package from which this asset was downloaded. If not then
it'll be null.
```c#
string Path { get; } 
```
The relative path with the asset extension. ie .wav becomes .vsnd
```c#
PublishSettings Publishing { get; } 
```
Access the asset publisher config.
```c#
string RelativePath { get; } 
```
The relative path as it is on disk (ie .wav not .vsnd)
```c#
AssetTags Tags { get; } 
```
Tags for this asset, for filtering purposes in the Asset Browser.
## Methods

```c#
void Compile( bool full) 
```
Forcibly recompile the asset.
```c#
ValueTask<bool> CompileIfNeededAsync( float timeout = 30) 
```
Returns a task that will resolve when the asset is compiled. If the asset is already compiled, do nothing. Does not support maps.
```c#
void Delete( ) 
```
Delete this asset. Will send the source and compiled files to the recycle bin.
```c#
void DumpThumbnail( ) 
```
Renders the thumbnail and then saves it to disk.
```c#
List<string> GetAdditionalRelatedFiles( ) 
```
Gets additional related files. This includes like .rect files for materials, all .fbx and .lxo files for models, etc.
```c#
Pixmap GetAssetThumb( bool generateIfNotInCache = true) 
```
Returns the asset preview thumbnail, with fallback to the asset type icon if there is no preview.
```c#
string GetCompiledFile( bool absolute = false) 
```
Returns the compiled file path, if the asset is compiled.
```c#
List<Asset> GetDependants( bool deep) 
```
Returns assets that depend/use this asset.
```c#
List<Asset> GetReferences( bool deep) 
```
Returns assets that this asset references/uses.
```c#
string GetSourceFile( bool absolute = false) 
```
Returns the source file path, if the sources are present.
```c#
List<string> GetUnrecognizedReferencePaths( ) 
```
Unrecognized reference paths listed by the data that could not be resolved into Asset*s
```c#
T LoadResource<T,>( ) 
```
Try to load this asset as aSandbox.Resourceof given type.
```c#
Resource LoadResource( Type resourceType) 
```
Try to load this asset as aSandbox.Resourceof given type.
```c#
void OpenInEditor( string nativeEditor = null) 
```
Try to open this asset in a supported editor.
You can specify nativeEditor to open in a specific editor.
```c#
void OverrideThumbnail( Pixmap pixmap) 
```
Override the Assets thumbnail with given one.
```c#
void RebuildThumbnail( bool startBuild = true) 
```
Delete existing cached thumbnail, optionally queuing for building a new one ASAP.
```c#
void RecordOpened( ) 
```
Tell asset system that this asset was opened. Sticks it on the recent opened list.
```c#
Pixmap RenderThumb( ) 
```
Immediately render a preview thumbnail for this asset, and return it.
```c#
bool SaveToDisk( GameResource obj) 
```
Save a game resource instance to disk. This is used internally by asset inspector and for asset creation.
```c#
bool SaveToMemory( GameResource obj, bool replace = true) 
```
Store a game resource instance to runtime cache, without saving to disk. This is used internally by asset inspector to apply asset edits.
```c#
bool TryLoadResource<T,>( out T obj) 
```
Try to load this asset as aSandbox.Resourceof given type.
```c#
override string ToString( ) 
```
OverridesObject.ToString
## Extensions

```c#
Task<bool> UploadVideo( byte[] contents, bool isThumbVideo, bool hidden = false, string tag = null, Callback progress = null, CancellationToken token = null) 
```
Upload a video for this package
## Nested Types

