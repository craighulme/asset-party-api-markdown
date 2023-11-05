# SpringJoint

## ```c#
Derives from PhysicsJoint
```

## Summary

A rope-like constraint that is has springy/bouncy.
## Properties

```c#
float MaxLength { get; set; } 
```
Maximum length it should be allowed to go
```c#
float MinLength { get; set; } 
```
Minimum length it should be allowed to go. At which point it acts a bit like a rod.
```c#
float ReferenceMass { get; set; } 
```
You shouldn't really ever need to change this, the default works out
what the reference mass should be based on actual physics.
```c#
PhysicsSpring SpringLinear { get; set; } 
```
How springy and tight the joint will be
