# DragData

## Derives from QObject

## Summary

Contains drag and drop data for tool widgets. SeeWidget.DragEvent.
## Constructors

```c#
DragData( ) 
```
No Summary
## Properties

```c#
string FileOrFolder { get; } 
```
The first file or folder in the drag data.
```c#
string[] Files { get; } 
```
All files and folders in the drag data.
```c#
bool HasFileOrFolder { get; } 
```
Whether the drag data has at least 1 file or folder.
```c#
string Html { get; set; } 
```
HTML data of the drag and drop event, if any.
```c#
object Object { get; set; } 
```
An object that can be used to pass drag and drop data
```c#
string Text { get; set; } 
```
Text data of the drag and drop event.
```c#
Uri Url { get; set; } 
```
URL data of the drag and drop event, if any.
