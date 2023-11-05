# BoxLayout

## 
```c#
Derives from Layout
```

## Summary

A widget layout. You can think of it as an invisible box of rows or columns, each one containing a widget, useful for automatic positioning and scaling.
## Methods

```c#
virtual T Add<T,>( T widget, int stretch = 0) 
```
No Summary
```c#
int GetCellStretch( int index) 
```
No Summary
```c#
void SetCellStretch( int index, int stretch) 
```
No Summary
```c#
void SetCellStretch( Widget widget, int stretch) 
```
No Summary
```c#
void SetCellStretch( Layout layout, int stretch) 
```
No Summary
```c#
override Layout Add( Layout layout) 
```
OverridesLayout.Add
```c#
override Layout Add( Layout layout, int stretch) 
```
OverridesLayout.Add
```c#
override void AddSpacingCell( float size) 
```
OverridesLayout.AddSpacingCellAdd a spacing item
```c#
override void AddStretchCell( int stretch = 0) 
```
OverridesLayout.AddStretchCellAdd a stretch item
