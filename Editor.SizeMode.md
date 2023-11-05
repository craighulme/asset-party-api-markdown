# SizeMode

## Derives from Enum

## Summary

Can grow beyond its size hint if necessary
## Fields

```c#
static SizeMode CanGrow = 1
```
Can grow beyond its size hint if necessary
```c#
static SizeMode CanShrink = 4
```
can shrink below its size hint if necessary.
```c#
static SizeMode Default = 5
```
Default size mode - CanGrow and CanShrink
```c#
static SizeMode Expand = 2
```
Should get as much space as possible.
```c#
static SizeMode Ignore = 8
```
Widget size is ignored, will get as much space as possible.
## Referencing Members

```c#
void Widget.SetSizeMode( SizeMode, SizeMode ) 
```
