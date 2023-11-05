# IMapViewDropTarget

## Is interface

## Summary

Provides an interface for dragging and droppingEditor.AssetorSandbox.Packageon a map view.
Use withMapEditor.CanDropAttributeto register your drop target for aPackage.TypeorSandbox.GameResourcetype.
## Methods

```c#
virtual void DragDropped( MapView view) 
```
Called when a dragged an asset or a package gets finally dropped on a Hammer view.
```c#
virtual void DragEnter( Asset asset, MapView view) 
```
An asset started being dragged over a Hammer view..
```c#
virtual void DragEnter( Package package, MapView view) 
```
An asset.party package started being dragged over a Hammer view..
```c#
virtual void DragLeave( MapView view) 
```
Called when a dragged an asset or a package gets dragged outside of a Hammer view.
This is a good spot to clean up any created nodes.
```c#
virtual void DragMove( MapView view) 
```
Called when the mouse cursor moves over a Hammer view while dragging an asset or a package.
