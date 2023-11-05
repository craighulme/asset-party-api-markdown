# Logger

## 
```c#
Derives from object
```

## Summary

Name of this logger.
## Constructors

```c#
Logger( string name) 
```
No Summary
## Properties

```c#
string Name { get; protected set; } 
```
Name of this logger.
## Methods

```c#
void Error( FormattableString message) 
```
Log an error. This is the most severe log level.
```c#
void Error( Exception exception, FormattableString message) 
```
Log an exception as an error, with given message override.
```c#
void Error( Exception exception, object message) 
```
Log an exception as an error, with given message override.
```c#
void Error( Exception exception) 
```
Log an exception as an error.
```c#
void Error( object message) 
```
Log an error. This is the most severe log level.
```c#
void Info( FormattableString message) 
```
Log some information. This is the default log severity level.
```c#
void Info( object message) 
```
Log some information. This is the default log severity level.
```c#
void Trace( FormattableString message) 
```
Log some information. This is least severe log level.
```c#
void Trace( object message) 
```
Log some information. This is least severe log level.
```c#
void Warning( FormattableString message) 
```
Log a warning. This is the second most severe log level.
```c#
void Warning( Exception exception, FormattableString message) 
```
Log an exception as a warning, with given message override.
```c#
void Warning( Exception exception, object message) 
```
Log an exception as a warning, with given message override.
```c#
void Warning( object message) 
```
Log a warning. This is the second most severe log level.
