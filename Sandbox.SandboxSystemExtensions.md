# SandboxSystemExtensions

## 
```c#
Derives from object
```

## Summary

Returns the angles of a uniformly random rotation.
## Methods

```c#
static Angles Angles( Random self) 
```
Returns the angles of a uniformly random rotation.
```c#
static string Base64Decode( string base64EncodedData) 
```
Convert from a base64 encoded string
```c#
static string Base64Encode( string plainText) 
```
Convert to a base64 encoded string
```c#
static int BitsSet( int i) 
```
Returns the number of bits set in an integer. This us usually used for flags to count
the amount of flags set.
```c#
static bool CheckValidationAttributes( PropertyInfo prop, object obj, out string[] errors, string name = null) 
```
Check all System.ComponentModel.DataAnnotations.ValidationAttributes on this property, and get the error messages if there are any.
```c#
static T Clamp<T,>( T input, T min, T max) 
```
Clamp a number between two values.
```c#
static Dictionary<TKey, TValue> Clone<TKey,TValue,>( Dictionary<TKey, TValue> dict) 
```
Clones the dictionary. Doesn't clone the values.
```c#
static Color Color( Random self) 
```
Returns a random Color
```c#
static string Columnize( string str, int maxLength, bool right = false) 
```
convert "string" into "string       " or "      string"
```c#
static bool Contains( string source, string toCheck, StringComparison comp) 
```
An extended Contains which takes a StringComparison.
```c#
static int Distance( string source, string target) 
```
Return the distance between two strings. Useful for ordering strings by similarity
```c#
static double Double( Random self, double min, double max) 
```
Returns a double between min and max
```c#
static double Double( Random self, double max = 1) 
```
Returns a random double between 0 and max (or 1)
```c#
static int FastHash( string str) 
```
Generate FNV-1a hash from given string.
```c#
static float Float( Random self, float min, float max) 
```
Returns a random float between min and max
```c#
static float Float( Random self, float max = 1) 
```
Returns a random float between 0 and max (or 1)
```c#
static Task ForEachTaskAsync<T,>( IEnumerable<T> source, Func<T, Task> body, int maxRunning = 8, CancellationToken token = null) 
```
Runs each task on this thread but only execute a set amount at a time
```c#
static string FormatBytes<T,>( T input, bool shortFormat = false) 
```
Given a number, will format as a memory value, ie 10gb, 4mb
```c#
static string FormatNumberShort( long num) 
```
"1500" becomes "1,500", "15 000" becomes "15K", "15 000 000" becomes "15KK", etc.
```c#
static string FormatNumberShort( ulong num) 
```
"1500" becomes "1,500", "15 000" becomes "15K", "15 000 000" becomes "15KK", etc.
```c#
static string FormatSeconds( long secs) 
```
Formats the given value in format "1w2d3h4m5s". Will not display 0 values.
```c#
static string FormatSeconds( ulong secs) 
```
Formats the given value in format "1w2d3h4m5s". Will not display 0 values.
```c#
static string FormatSecondsLong( long secs) 
```
Formats the given value in format "4 weeks, 3 days, 2 hours and 1 minutes".
Will not display 0 values. Will not display seconds if value is more than 1 hour.
```c#
static string FormatSecondsLong( ulong secs) 
```
Formats the given value in format "4 weeks, 3 days, 2 hours and 1 minutes".
Will not display 0 values. Will not display seconds if value is more than 1 hour.
```c#
static string FormatWithSuffix( int num) 
```
Change 1 to 1st, 2 to 2nd etc
```c#
static T FromArray<T,>( Random self, T[] array, T defVal = null) 
```
Returns a random value in an array
```c#
static long FromBase36( string input) 
```
Decode the Base36 Encoded string into a number
```c#
static T FromList<T,>( Random self, List<T> array, T defVal = null) 
```
Returns a random value in a list
```c#
static float Gaussian( Random self, float mean = 0, float stdDev = 1) 
```
Sample from a Gaussian distribution with a given mean and standard deviation.
```c#
static Vector2 Gaussian2D( Random self, Vector2? mean = null, Vector2? stdDev = null) 
```
Sample from a 2D Gaussian distribution with a given mean and standard deviation.
```c#
static Vector3 Gaussian3D( Random self, Vector3? mean = null, Vector3? stdDev = null) 
```
Sample from a 3D Gaussian distribution with a given mean and standard deviation.
```c#
static Vector4 Gaussian4D( Random self, Vector4? mean = null, Vector4? stdDev = null) 
```
Sample from a 4D Gaussian distribution with a given mean and standard deviation.
```c#
static T GetAttributeOfType<T,>( Enum enumVal) 
```
Gets an attribute on an enum field value
```c#
static int GetEpoch( DateTime d) 
```
Returns the UNIX time stamp - number of seconds since 1st of January, 1970.
```c#
static TValue GetOrCreate<TKey,TValue,>( Dictionary<TKey, TValue> dict, TKey key) 
```
If the key doesn't exist it is created and returned
```c#
static TValue GetValueOrDefault<TKey,TValue,>( Dictionary<TKey, TValue> dict, TKey key, TValue defaultValue = null) 
```
Return value at given key, if it doesn't exist, return given default value instead.
```c#
static int Int( Random self, int min, int max) 
```
Returns a random int between min and max (inclusive)
```c#
static int Int( Random self, int max) 
```
Returns a random int between 0 and max (inclusive)
```c#
static bool IsBasedOnGenericType( Type src, Type test) 
```
Returns if this type is based on a given generic type.
```c#
static bool IsInitOnly( PropertyInfo property) 
```
Determine if this property is init-only.
```c#
static bool IsValid( IValid obj) 
```
Returns false ifSandbox.IValidobject is null or ifIValid.IsValidreturns false.
```c#
static string KiloFormat( int num) 
```
Format a large number into "1045M", "56K"
```c#
static string KiloFormat( long num) 
```
Format a large number into "1045M", "56K"
```c#
static string NormalizeFilename( string str, bool enforceInitialSlash = true) 
```
Puts a filename into the format /path/filename.ext (from path\FileName.EXT)
```c#
static string Plural( int a, string single, string plural) 
```
Return single if 1 else plural
```c#
static string QuoteSafe( string str, bool optional = false) 
```
Puts quote marks around a string. Internal quotes are backslashed.
```c#
static Angles ReadAngles( BinaryReader reader) 
```
Read an angles object from given binary reader.
```c#
static Color ReadColor( BinaryReader reader) 
```
Read a color from binary reader.
```c#
static string ReadNullTerminatedString( Stream stream, long offset) 
```
Read a null terminated string from the stream, at given offset.
```c#
static Ray ReadRay( BinaryReader reader) 
```
Read aRayfrom given binary reader.
```c#
static Rotation ReadRotation( BinaryReader reader) 
```
Read a rotation from given binary reader.
```c#
static Transform ReadTransform( BinaryReader reader) 
```
Read a transform from given binary reader.
```c#
static Vector2 ReadVector2( BinaryReader reader) 
```
Read a vector2 from given binary reader.
```c#
static Vector3 ReadVector3( BinaryReader reader) 
```
Read a vector3 from given binary reader.
```c#
static string RemoveBadCharacters( string str) 
```
Removes bad, invisible characters that are commonly used to exploit.https://en.wikipedia.org/wiki/Zero-width_non-joiner
```c#
static Rotation Rotation( Random self) 
```
Returns a uniformly random rotation.
```c#
static string SimplifyPath( string str) 
```
Gets rid of ../'s (from /path/folder/../file.txt to /path/file.txt)
```c#
static string Snippet( string source, string find, int padding) 
```
Given a large string, find all occurrences of a substring and return them with padding.
This is useful in situations where you're searching for a word in a hug body of text, and
want to show how it's used without displaying the whole text.
```c#
static string[] SplitQuotesStrings( string input) 
```
in  : I am "splitting a" string "because it's fun "
out : ["I", "am", "splitting a", "string", "because it's fun"]
```c#
static string ToBase36<T,>( T i) 
```
Encode the given number into a Base36 string
```c#
static bool ToBool( string str) 
```
Try to convert to bool. Inputs can be true, false, yes, no, 0, 1, null (caps insensitive)
```c#
static DateTime ToDateTime( int seconds) 
```
Converts UNIX time stamp to a DateTime object.
```c#
static DateTime ToDateTime( long seconds) 
```
Converts UNIX time stamp to a DateTime object.
```c#
static Decimal ToDecimal( string str, Decimal Default = 0) 
```
128-bit data type that returns sane results for almost any input.
All other numeric types can cast from this.
```c#
static float ToFloat( string str, float Default = 0) 
```
Convert to float, if not then return Default
```c#
static int ToInt( string str, int Default = 0) 
```
Convert to int, if not then return Default
```c#
static long ToLong( string str, long Default = 0) 
```
Convert to long, if not then return Default
```c#
static string ToRelativeTimeString( DateTime dateTime) 
```
No Summary
```c#
static string ToRelativeTimeString( TimeSpan span) 
```
No Summary
```c#
static string ToTitleCase( string source) 
```
Convert a variable name to something more user friendly.
```c#
static object ToType( string str, Type t) 
```
Try to politely convert from a string to another type
```c#
static uint ToUInt( string str, int Default = 0) 
```
Convert to uint, if not then return Default
```c#
static ulong ToULong( string str, ulong Default = 0) 
```
Convert to ulong, if not then return Default
```c#
static string TrimQuoted( string str, bool ignoreSurroundingSpaces = false) 
```
The string might start and end in quotes ( ", ' ), remove those if that is the case.
```c#
static string Truncate( string str, int maxLength, string appendage = null) 
```
If the string is longer than this amount of characters then truncate it
If appendage is defined, it will be appended to the end of truncated strings (ie, "..")
```c#
static string TruncateFilename( string str, int maxLength, string appendage = null) 
```
If the string is longer than this amount of characters then truncate it
If appendage is defined, it will be appended to the end of truncated strings (ie, "..")
```c#
static bool TryToType( string str, Type t, out object Value) 
```
Try to politely convert from a string to another type
```c#
static int UnsignedMod( int a, int b) 
```
Does what you expected to happen when you did "a % b", that is, handles negativeavalues by returning a positive number from the end.
```c#
static Vector2 VectorInCircle( Random self, float radius = 1) 
```
Uniformly samples a 2D position from all points with distance at mostradiusfrom the origin.
```c#
static Vector3 VectorInCube( Random self, float extents = 1) 
```
Uniformly samples a 3D position from a cube with coordinates in the range -extentsto +extents.
```c#
static Vector3 VectorInSphere( Random self, float radius = 1) 
```
Uniformly samples a 3D position from all points with distance at mostradiusfrom the origin.
```c#
static Vector2 VectorInSquare( Random self, float extents = 1) 
```
Uniformly samples a 2D position from a square with coordinates in the range -extentsto +extents.
```c#
static bool WildcardMatch( string str, string wildcard) 
```
Returns true if this string matches a wildcard match. Check is case insensitive.
```c#
static void Write( BinaryWriter writer, Vector3 v) 
```
Write aVector3to the binary writer.
```c#
static void Write( BinaryWriter writer, Vector2 v) 
```
Write aVector2to the binary writer.
```c#
static void Write( BinaryWriter writer, Angles v) 
```
Write aSandboxSystemExtensions.Anglesto the binary writer.
```c#
static void Write( BinaryWriter writer, Rotation r) 
```
Write aSandboxSystemExtensions.Rotationto the binary writer.
```c#
static void Write( BinaryWriter writer, Ray v) 
```
Write aRayto the binary writer.
```c#
static void Write( BinaryWriter writer, Transform v) 
```
Write this transform to a System.IO.BinaryWriter.
```c#
static void Write( BinaryWriter writer, Color v) 
```
Write this color to a binary writer.
