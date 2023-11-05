# AudioMaterial

## Derives from GameResource

## Summary

An audio material defines the acoustic properties of a surface.
The acoustic material properties are specified for three frequency bands with center frequencies of 400 Hz, 2.5 KHz, and 15 KHz.
## Constructors

```c#
AudioMaterial( ) 
```
No Summary
## Properties

```c#
Vector3 Absorption { get; set; } 
```
Fraction of sound energy absorbed at low, middle, high frequencies. Between 0.0 and 1.0.
```c#
float Scattering { get; set; } 
```
Fraction of sound energy scattered in a random direction on reflection. Between 0.0 (pure specular) and 1.0 (pure diffuse)
```c#
Vector3 Transmission { get; set; } 
```
Fraction of sound energy transmitted through at low, middle, high frequencies. Between 0.0 and 1.0.
