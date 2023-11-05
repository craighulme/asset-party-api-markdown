# Pixmap

## Derives from object

## Summary

A pixel map, or just a simple image.
## Constructors

```c#
Pixmap( int width, int height) 
```
Create a new empty pixel map. It can then be drawn to via theEditor.Paintclass, like so:var myPixMap = new Pixmap( 16, 16 );

 Paint.Target( myPixMap );
  Paint.Antialiasing = true;
  Paint.ClearPen();
  Paint.SetBrush( Color.Red );
  Paint.DrawRect( new Rect( 0, myPixMap.Size ), 2 );
 Paint.Target( null );
```c#
Pixmap( Vector2 size) 
```
Create a new empty pixel map. It can then be drawn to via theEditor.Paintclass, like so:var myPixMap = new Pixmap( 16, 16 );

 Paint.Target( myPixMap );
  Paint.Antialiasing = true;
  Paint.ClearPen();
  Paint.SetBrush( Color.Red );
  Paint.DrawRect( new Rect( 0, myPixMap.Size ), 2 );
 Paint.Target( null );
## Properties

```c#
bool HasAlpha { get; } 
```
Whether this pixel map supports the alpha channel.
```c#
float Height { get; } 
```
Height of the pixel map.
```c#
Vector2 Size { get; } 
```
THe size of this pixel map.
```c#
float Width { get; } 
```
Width of the pixel map.
## Methods

```c#
static Pixmap FromFile( string filename) 
```
Load an image from a file on disk, specifically from "core/tools/images".
```c#
void Clear( Color color) 
```
Fill the pixel map with given color.
```c#
byte[] GetBmp( int quality) 
```
Returns the raw bytes of a BMP file that contains this pixel maps image.
Internally writes and deletes a file, so be careful using it often.
```c#
byte[] GetJpeg( int quality) 
```
Returns the raw bytes of a JPEG file that contains this pixel maps image.
Internally writes and deletes a file, so be careful using it often.
```c#
byte[] GetPng( ) 
```
Returns the raw bytes of a PNG file that contains this pixel maps image.
Internally writes and deletes a file, so be careful using it often.
```c#
Pixmap Resize( Vector2 size) 
```
Returns a new pixel map that contains resized version of this image with given dimensions.
Will try to preserve aspect ratio.
```c#
Pixmap Resize( int x, int y) 
```
Returns a new pixel map that contains resized version of this image with given dimensions.
Will try to preserve aspect ratio.
```c#
bool SaveJpg( string filename, int quality = 70) 
```
Save the pixel map as a JPEG file at given location.
```c#
bool SavePng( string filename) 
```
Save the pixel map as a PNG file at given location.
```c#
void Scroll( int x, int y, Rect r) 
```
Duplicate a sub-rectangle of the image at re-draw it at given coordinates.
```c#
void Scroll( int x, int y) 
```
Duplicate the entire image and re-draw it at given coordinates.
```c#
bool UpdateFromPixels( ReadOnlySpan<byte> data, int width, int height, ImageFormat format = 12) 
```
Writes raw pixels to the pixel map. Only BGRA8888 is currently supported.
```c#
bool UpdateFromPixels( ReadOnlySpan<byte> data, Vector2 size, ImageFormat format = 12) 
```
Writes raw pixels to the pixel map. Only BGRA8888 is currently supported.
