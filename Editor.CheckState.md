# CheckState

## ```c#
Derives from Enum
```

## Summary

Check state of aEditor.CheckBox.
## Fields

```c#
static CheckState Off = 0
```
The checkbox is not checked.
```c#
static CheckState On = 2
```
The checkbox is checked.
```c#
static CheckState Partial = 1
```
Partial. This is useful in cases when representing multiple objects,
with a boolean value where some are set to true, and others to false.
## Referencing Members

```c#
protected virtual void CheckBox.OnStateChanged( CheckState ) 
```
```c#
CheckState = CheckBox.State { get; set; } 
```
```c#
Action<CheckState> = CheckBox.StateChanged
```
