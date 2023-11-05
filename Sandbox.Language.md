# Language

## 
```c#
Derives from object
```

## Summary

Allows access to translated phrases, allowing the translation of gamemodes etc
## Properties

```c#
static LanguageInformation Current { get; } 
```
Information about the current selected language. Will default to English if the current language isn't found.
```c#
static string SelectedCode { get; set; } 
```
The abbreviation for the language the user wants. This is set by the user in the options menu.
## Methods

```c#
static string GetPhrase( string textToken) 
```
Lookup a phrase
```c#
static string GetPhrase( string textToken, Dictionary<string, object> data) 
```
Look up a phrase
