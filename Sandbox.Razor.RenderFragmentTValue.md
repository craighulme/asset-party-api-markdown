# RenderFragment<TValue>

## ```c#
Derives from MulticastDelegate
```

## Summary

Represents a segment of UI content for an object of typeTValue, implemented as
a function that returns aRazor.RenderFragment.
## Type Parameters

```c#
TValue
```
No Summary
## Constructors

```c#
RenderFragment( object object, IntPtr method) 
```
No Summary
## Methods

```c#
virtual IAsyncResult BeginInvoke( TValue value, AsyncCallback callback, object object) 
```
No Summary
```c#
virtual RenderFragment EndInvoke( IAsyncResult result) 
```
No Summary
```c#
virtual RenderFragment Invoke( TValue value) 
```
No Summary
