# HistoryList<T>

## Derives from object

## Summary

A helper class to store a list of strings, which can then be navigated around, saved, restored
## Type Parameters

```c#
T
```
No Summary
## Constructors

```c#
HistoryList( ) 
```
No Summary
## Fields

```c#
Action<T> OnNavigate
```
Called when navigations successfully happened.
## Properties

```c#
bool CanGoBack { get; } 
```
No Summary
```c#
bool CanGoForward { get; } 
```
No Summary
```c#
T Current { get; } 
```
No Summary
```c#
bool Debug { get; set; } 
```
Print debug information on navigation
```c#
int MaxItems { get; set; } 
```
The maximum history length
```c#
string StateCookie { get; set; } 
```
No Summary
## Methods

```c#
void Add( T text) 
```
Navigate to the previous item in the list, removes any items after the current position.
```c#
void Clear( ) 
```
No Summary
```c#
bool Navigate( int delta) 
```
Navigate to delta positions from the current position. For example, -1 is backwards.
Returns false if nothing changed.
