# VisualStudio

## ```c#
Implements ICodeEditor
```

## Summary

ImplementsICodeEditor.IsInstalledWhether or not this editor is installed.
## Constructors

```c#
VisualStudio( ) 
```
No Summary
## Methods

```c#
virtual bool IsInstalled( ) 
```
ImplementsICodeEditor.IsInstalledWhether or not this editor is installed.
```c#
virtual void OpenAddon( LocalProject addon) 
```
ImplementsICodeEditor.OpenAddonOpen given addon in the editor.
```c#
virtual void OpenFile( string path, int? line, int? column) 
```
ImplementsICodeEditor.OpenFileOpens a file in the editor, optionally at a line and column.
```c#
virtual void OpenSolution( ) 
```
ImplementsICodeEditor.OpenSolutionOpen the solution of all sandbox projects
