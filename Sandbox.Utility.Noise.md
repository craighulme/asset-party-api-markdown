# Noise

## ```c#
Derives from object
```

## Summary

Provides access to coherent noise utilities.All of these functions should return between -1 and 1.
## Methods

```c#
static float Fbm( int octaves, float x, float y = 0, float z = 0) 
```
Fractional Brownian Motionnoise, a.k.a. Fractal Perlin noise.
```c#
static Vector3 FbmVector( int octaves, float x, float y = 0) 
```
Fractional Brownian Motionnoise, a.k.a. Fractal Perlin noise.
```c#
static float Perlin( float x) 
```
A "one dimensional"Perlin noisefunction.
```c#
static float Perlin( float x, float y) 
```
2DPerlin noisefunction.
```c#
static float Perlin( float x, float y, float z) 
```
3DPerlin noisefunction.
```c#
static float Simplex( float x) 
```
A "one dimensional"Simplex noisefunction.
```c#
static float Simplex( float x, float y) 
```
2DSimplex noisefunction.
```c#
static float Simplex( float x, float y, float z) 
```
3DSimplex noisefunction.
