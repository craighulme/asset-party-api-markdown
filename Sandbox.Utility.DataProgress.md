# DataProgress

## 
```c#
Derives from ValueType
```

## Summary

For providing a callback to describe the progress of doing something with some kind of block of data
## Properties

```c#
long DeltaBytes { get; set; } 
```
No Summary
```c#
long ProgressBytes { get; set; } 
```
No Summary
```c#
float ProgressDelta { get; } 
```
No Summary
```c#
long TotalBytes { get; set; } 
```
No Summary
## Nested Types

## Referencing Members

```c#
virtual IAsyncResult = Callback.BeginInvoke( DataProgress, AsyncCallback, object ) 
```
```c#
virtual void Callback.Invoke( DataProgress ) 
```
