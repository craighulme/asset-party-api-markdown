# PropertyEditorWidget

## ```c#
Derives from Widget
```

## Summary

The DisplayInfo from the PropertyInfo (if applicable)
## Constructors

```c#
PropertyEditorWidget( Widget parent) 
```
No Summary
```c#
PropertyEditorWidget( ) 
```
No Summary
## Properties

```c#
protected DisplayInfo? PropertyDisplay { get; set; } 
```
The DisplayInfo from the PropertyInfo (if applicable)
## Methods

```c#
virtual void OnReady( ) 
```
Called after all display info attributes are applied from the property. This doesn't mean that
the current value has been set yet.
```c#
virtual void SetPropertyDisplayInfo( DisplayInfo display) 
```
If we have applicable property info this will be set via this call automatically
## Inheriting Types

