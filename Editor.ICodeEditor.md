# ICodeEditor

## ```c#
Is interface
```

## Summary

Interface for editors to open code files.
Any class that implements this interface is automatically added to the list.
An editor is only enabled ifICodeEditor.IsInstalledreturns true.Decorate your implementation with aTitleAttribute.
## Methods

```c#
abstract bool IsInstalled( ) 
```
Whether or not this editor is installed.
```c#
abstract void OpenAddon( LocalProject addon) 
```
Open given addon in the editor.
```c#
abstract void OpenFile( string path, int? line = null, int? column = null) 
```
Opens a file in the editor, optionally at a line and column.
```c#
abstract void OpenSolution( ) 
```
Open the solution of all sandbox projects
