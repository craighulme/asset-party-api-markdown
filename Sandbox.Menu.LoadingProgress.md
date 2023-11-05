# LoadingProgress

## 
```c#
Derives from ValueType
```

## Summary

A value between 0 and 1, to show a progress bar
## Properties

```c#
double Fraction { get; set; } 
```
A value between 0 and 1, to show a progress bar
```c#
double Mbps { get; set; } 
```
The current transfer rate in Megabits per second. 0 is none.
```c#
double Percent { get; } 
```
Delta multipled by 100
```c#
string Subtitle { get; set; } 
```
No Summary
```c#
string Title { get; set; } 
```
No Summary
## Referencing Members

```c#
abstract void ILoadingScreenPanel.OnLoadingProgress( LoadingProgress ) 
```
```c#
virtual void DefaultLoadingPanel.OnLoadingProgress( LoadingProgress ) 
```
```c#
LoadingProgress = DefaultLoadingPanel.Progress
```
