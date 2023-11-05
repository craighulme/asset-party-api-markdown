# CloudAsset

## ```c#
Derives from object
```

## Summary

Install multiple packages. Will popup a progress window
## Constructors

```c#
CloudAsset( ) 
```
No Summary
## Methods

```c#
static Task<bool> Install( string windowTitle, IEnumerable<string> packages) 
```
Install multiple packages. Will popup a progress window
```c#
static Task InstallSingle( string ident) 
```
Install a cloud asset by ident
