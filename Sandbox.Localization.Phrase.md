# Phrase

## ```c#
Derives from object
```

## Summary

A translated string. ie "Hello World".
It might also have variables, ie "Hello ".
Todo support for conditionals and plurals
## Constructors

```c#
Phrase( string value) 
```
Create a SmartString from a phrase.
## Methods

```c#
string Render( ) 
```
Render with no data - basically just returns Value
```c#
string Render( Dictionary<string, object> data) 
```
Render with variables
