# RenderTreeBuilder

## 
```c#
Derives from object
```

## Summary

This is a tree renderer for panels. If we ever use razor on other ui we'll want to make a copy of
this class and do the specific things to that.
## Methods

```c#
virtual void AddAttribute( int sequence, string attrName, object value) 
```
Handles "style" and "class" attributes..
```c#
virtual void AddAttribute<T,>( int sequence, Action<T> value) 
```
<Icon OnSomething=@Function></Icon>
```c#
virtual void AddAttribute( int sequence, string attrName, Action value) 
```
Handles @onclick=@( () => DoSomething( "boobies" ) )
```c#
virtual void AddAttribute( int sequence, string attrName, Func<Task> value) 
```
Handles @onclick=@( () => await DoSomethingAsync( "boobies" ) )
```c#
virtual void AddAttribute( int sequence, string attrName, Action<PanelEvent> value) 
```
Handles @onclick=@( ( PanelEvent e ) => DoSomething( e.This, "boobies" ) )
```c#
virtual void AddAttribute<T,>( int sequence, object value, Action<T> setter) 
```
Called to set attributes on a panel directly
```c#
virtual void AddBind<T,>( int sequence, string propertyName, Func<T> get, Action<T> set) 
```
Called to set attributes on a panel directly
```c#
virtual void AddContent<T,>( int sequence, T content) 
```
Handles text content within an element
```c#
virtual void AddLocation( string filename, int line, int column) 
```
Add the current source location. Used to record in which file the element was created.
```c#
virtual void AddStyleDefinitions( int sequence, string styles) 
```
Styles from a style block
```c#
virtual void CloseElement( ) 
```
Finish working on this element
```c#
virtual void OpenElement( int sequence, string elementName) 
```
Start working on this element
```c#
void AddMarkupContent( int sequence, string markupContent) 
```
Add markup to the current element
```c#
void AddReferenceCapture<T,>( int sequence, T current, Action<T> value) 
```
Implements @ref
```c#
void OpenElement<T,>( int sequence) 
```
Create a panel of type T
```c#
void SetRenderFragment<T,>( Action<T, RenderFragment> setter, RenderFragment builder) 
```
No Summary
```c#
void SetRenderFragmentWithContext<T,U,>( Func<T, RenderFragment<U>> getter, Action<T, RenderFragment<U>> setter, RenderFragment<U> builder) 
```
No Summary
