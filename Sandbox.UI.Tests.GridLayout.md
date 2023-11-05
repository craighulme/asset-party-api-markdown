# GridLayout

## 
```c#
Derives from object
```

## Summary

Should we update Columns automatically?
## Constructors

```c#
GridLayout( ) 
```
No Summary
## Properties

```c#
bool AutoColumns { get; set; } 
```
Should we update Columns automatically?
```c#
int Columns { get; set; } 
```
How many columns should we have?
```c#
Length ItemHeight { get; set; } 
```
The fixed height of each item.
```c#
Length ItemWidth { get; set; } 
```
The fixed width of each item. If it is lower than 0 then we'll stretch to fill the size.
```c#
Justify Justify { get; protected set; } 
```
How columns should be justified
```c#
Rect Rect { get; protected set; } 
```
The Rect of this layout. Set via Update.
```c#
float ScrollOffset { get; protected set; } 
```
Where the top of the visible space is
## Methods

```c#
float GetHeight( int count) 
```
Get the full height if we have this many items
```c#
Rect GetPosition( int index) 
```
Get the position of this cell
```c#
void GetVisibleRange( out int firstIndex, out int lastIndex) 
```
Get the range of cells that are visible
```c#
void Position( int index, Panel panel) 
```
Move this panel into the position. This will set the Left/Top/Width/Height on the panel
```c#
bool Update( Box box, float scaleFromScreen, float scrollOffset, Justify justify) 
```
Update specifics of this layout. Returns true if we're dirty.
