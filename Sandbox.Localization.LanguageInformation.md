# LanguageInformation

## Derives from object

## Summary

ISO 639-1 code of the language, with optional ISO 3166-1 alpha-2 country specifiers. (for example "en-GB" for British English)
## Constructors

```c#
LanguageInformation( string title, string abbreviation, string parent = null, bool rightToLeft = false) 
```
No Summary
## Properties

```c#
string Abbreviation { get; } 
```
ISO 639-1 code of the language, with optional ISO 3166-1 alpha-2 country specifiers. (for example "en-GB" for British English)
```c#
string Parent { get; } 
```
If set, theLanguageInformation.Abbreviationof the parent language. For example, Pirate English is based on English.
```c#
bool RightToLeft { get; } 
```
Whether the language is typed right to left, such as the Arabic language.
```c#
string Title { get; } 
```
Title of the localization language.
