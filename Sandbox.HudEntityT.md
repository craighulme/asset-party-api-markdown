# HudEntity<T>

## ```c#
Derives from Entity
```

## Summary

A base HUD entity that lets you define which type of RootPanel to create.
## Type Parameters

```c#
T is RootPanel, new(), 
```
No Summary
## Constructors

```c#
HudEntity( ) 
```
No Summary
## Properties

```c#
T RootPanel { get; set; } 
```
No Summary
## Methods

```c#
virtual void CreateRootPanel( ) 
```
Create the root panel, T
```c#
protected override void OnDestroy( ) 
```
OverridesEntity.OnDestroyCalled when the entity was destroyed. This is not the same as the class destructor.
