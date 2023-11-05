# FilmGrainSettings

## Derives from object

## Summary

How intense the grain output should be. This is a value
from 0->1
## Constructors

```c#
FilmGrainSettings( ) 
```
No Summary
## Properties

```c#
float Intensity { get; set; } 
```
How intense the grain output should be. This is a value
from 0->1
```c#
float Response { get; set; } 
```
How responsive the grain should be to light values. A result
of 0 will lead to the grain being very responsive everywhere
whereas a value of 1 will lead to the grain only being responsive in darker
areas.
The range is from 0->1
