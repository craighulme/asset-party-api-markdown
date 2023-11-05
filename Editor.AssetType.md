# AssetType

## Derives from object

## Summary

All currently registered asset types, including the base types such as models, etc.
## Constructors

```c#
AssetType( ) 
```
No Summary
## Properties

```c#
static IReadOnlyCollection<AssetType> All { get; } 
```
All currently registered asset types, including the base types such as models, etc.
```c#
static AssetType Animation { get; protected set; } 
```
Animation (.vanim) asset type.
```c#
static AssetType AnimationGraph { get; protected set; } 
```
Animation Graph (.vanmgrph) asset type.
```c#
static AssetType ImageFile { get; protected set; } 
```
Image source (.png or .jpg) asset type.
```c#
static AssetType MapFile { get; protected set; } 
```
A map (.vmap) asset type.
```c#
static AssetType Material { get; protected set; } 
```
Material (.vmat) asset type.
```c#
static AssetType Model { get; protected set; } 
```
Model (.vmdl) asset type.
```c#
static AssetType ParticleSystem { get; protected set; } 
```
Particle System (.vpcf) asset type.
```c#
static AssetType Shader { get; protected set; } 
```
Shader (.shader) asset type.
```c#
static AssetType SoundEvent { get; protected set; } 
```
A sound event
```c#
static AssetType SoundFile { get; protected set; } 
```
Sound (.wav, .ogg or .mp3) asset type.
```c#
static AssetType Soundscape { get; protected set; } 
```
A soundscape
```c#
static AssetType Texture { get; protected set; } 
```
Texture (.vtex) asset type.
```c#
bool CanBePublished { get; } 
```
True if this is an asset type that can be published on asset.party
```c#
string Category { get; } 
```
Category of this asset type, for grouping in UI.
```c#
string FileExtension { get; } 
```
Primary file extension for this asset type.
```c#
string FriendlyName { get; } 
```
Name of the asset type for UI purposes.
```c#
bool HasVideoThumbnails { get; } 
```
True if we want to upload video thumbnails when we publish this asset type
```c#
bool HiddenByDefault { get; } 
```
This asset type is hidden by default from asset browser, etc.
```c#
Pixmap Icon128 { get; } 
```
128x128 icon for this asset type.
```c#
Pixmap Icon16 { get; } 
```
16x16 icon for this asset type.
```c#
Pixmap Icon256 { get; } 
```
256x256 icon for this asset type.
```c#
Pixmap Icon64 { get; } 
```
64x64 icon for this asset type.
```c#
bool IsGameResource { get; } 
```
Whether this asset type is a custom game resource or not.
```c#
bool PrefersIconThumbnail { get; } 
```
Use asset type icon, over any preview image.
## Methods

```c#
static AssetType Find( string name, bool allowPartials = false) 
```
Find an asset type by name or extension match.
```c#
static AssetType FromType( Type t) 
```
For a type (ie Texture, Material, Surface) return the appropriate AssetType.
Returns null if can't resolve.
```c#
override string ToString( ) 
```
OverridesObject.ToString
