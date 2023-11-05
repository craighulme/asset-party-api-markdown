# ThumbnailRendererAttribute

## 
```c#
Derives from Attribute
```

## Summary

Should target a static method likepublic static Pixmap RenderThumbnail( Asset thumbnail )where the method returns a thumbnail for that asset type.
This kind of sucks I don't like it.
## Constructors

```c#
ThumbnailRendererAttribute( ) 
```
No Summary
## Properties

```c#
int Priority { get; set; } 
```
The priority of this callback. Higher gets called first.
