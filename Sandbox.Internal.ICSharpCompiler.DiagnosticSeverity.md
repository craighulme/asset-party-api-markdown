# DiagnosticSeverity

## ```c#
Derives from Enum
```

## Summary

The severity of an output from the compiler
## Fields

```c#
static DiagnosticSeverity Error = 3
```
Something not allowed by the rules of the language or other authority.
```c#
static DiagnosticSeverity Hidden = 0
```
Something that is an issue, as determined by some authority,
but is not surfaced through normal means.
There may be different mechanisms that act on these issues.
```c#
static DiagnosticSeverity Info = 1
```
Information that does not indicate a problem (i.e. not prescriptive).
```c#
static DiagnosticSeverity Warning = 2
```
Something suspicious but allowed.
## Referencing Members

```c#
DiagnosticSeverity = Diagnostic.Severity
```
