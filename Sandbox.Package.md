# Package

## ```c#
Derives from object
```

## Summary

Represents an asset onAsset Party.
## Constructors

```c#
Package( ) 
```
No Summary
## Properties

```c#
virtual bool IsRemote { get; } 
```
Whether this is a remote or a locally installed package.
```c#
virtual IRevision Revision { get; } 
```
Information about the current package revision/version.
```c#
virtual string[] Tags { get; set; } 
```
List of tags for this package.
```c#
int ApiVersion { get; set; } 
```
For game extension compatibility. Game targeting extensions are only compatible with that game
if the API Versions match.
```c#
bool Archived { get; set; } 
```
Whether this package is archived or not.
```c#
bool CanEdit { get; } 
```
True if we're a member of this package's organization.
```c#
int Collections { get; set; } 
```
How many collections we're in (roughly)
```c#
DateTimeOffset Created { get; set; } 
```
When the package was originally created.
```c#
string Description { get; set; } 
```
Full description of the package.
```c#
string[] EditorReferences { get; set; } 
```
List of packages that this package depended on during editing.
```c#
int EngineVersion { get; set; } 
```
Engine version this package was uploaded with.
This is useful for when the base game undergoes large API changes.
```c#
int Favourited { get; set; } 
```
Number of players who added this package to their favourites.
```c#
string FullIdent { get; } 
```
Full unique identity of this package.
```c#
string Ident { get; set; } 
```
Unique identity of this package within itsorganization..
```c#
PackageInteraction Interaction { get; set; } 
```
Describes the authenticated user's interactions with this package. This is only available
clientside for specific users in order to show things like play history state, favourite
status and whether they have rated the item or not.
```c#
bool IsFavourite { get; } 
```
True if this asset is in our favourite list.
```c#
List<string> MapList { get; } 
```
No Summary
```c#
MapSelect MapSelectionMode { get; } 
```
No Summary
```c#
Organization Org { get; set; } 
```
The owner of this package.
```c#
string[] PackageReferences { get; set; } 
```
List of packages that this package depends on. These will be downloaded and installed when
installing this package.
```c#
List<GameSetting> PackageSettings { get; } 
```
Meta used by Game and Extension Packages to allow some configuration
```c#
Type PackageType { get; set; } 
```
What kind of package it is.
```c#
bool Public { get; set; } 
```
Whether this package is public or hidden.
```c#
int Referenced { get; set; } 
```
How many packages we're referenced by (roughly)
```c#
int Referencing { get; set; } 
```
How many packages we're referencing (roughly)
```c#
Screenshot[] Screenshots { get; set; } 
```
A list of screenshots
```c#
string Source { get; set; } 
```
Link to this package's sources, if set.
```c#
string Summary { get; set; } 
```
A short summary of the package.
```c#
bool SupportsSavedGames { get; } 
```
Meta used by Game Packages to determine if saved games are supported
```c#
string Thumb { get; set; } 
```
Link to the thumbnail image of this package.
```c#
string Title { get; set; } 
```
A "nice" name of this package, which will be shown to players in UI.
```c#
DateTimeOffset Updated { get; set; } 
```
When the entry was last updated. If these are different between packages
then something updated on the backend.
```c#
string Url { get; } 
```
A link to this asset on Asset Party.
```c#
PackageUsageStats Usage { get; set; } 
```
Statistics for user interactions with this package
```c#
string VideoThumb { get; set; } 
```
Link to the thumbnail video of this package.
```c#
int VotesDown { get; set; } 
```
Number of players who voted this package down.
```c#
int VotesUp { get; set; } 
```
Number of players who voted this package up.
## Methods

```c#
static Task<Package> Fetch( string identString, bool partial) 
```
Find package information
```c#
static Task<Package> FetchAsync( string identString, bool partial) 
```
Find package information
```c#
static Task<Package> FetchAsync( string identString, bool partial, bool useCache) 
```
Find package information
```c#
static Task<FindResult> FindAsync( string query, int take = 200, int skip = 0, CancellationToken token = null) 
```
Retrieve a list of packages
```c#
static string GetCachedTitle( string ident) 
```
If we have this package information, try to get its name
```c#
static Task<ListResult> ListAsync( int amountPerGroup, CancellationToken token = null) 
```
Retrieve a list of packages, organised into groups, for discovery
```c#
static IEnumerable<Package> SortByReferences( IEnumerable<Package> unordered) 
```
Sort the given list of packages so that referenced packages are ordered before the packages that reference them.
```c#
static IEnumerable<T> SortByReferences<T,>( IEnumerable<T> unordered, Func<T, Package> getPackageFunc) 
```
Sort the given list of items so that referenced packages are ordered before the packages that reference them.
```c#
static bool TryGetCached( string identString, out Package package, bool allowPartial = true) 
```
Find package information
```c#
static bool TryParseIdent( string ident, out ValueTuple<string, string, int, bool> parsed) 
```
Parse a package ident into parts. There are a few different formats you can pass to this.org/packageorg.packageorg.package#version
-https://asset.party/org/package-https://asset.party/org/package#versionIf package version isn't specified version will be 0
```c#
virtual T GetMeta<T,>( string keyName, T defaultValue = null) 
```
Get metadata value from this package for given key. This will be specific to eachPackage.Type.
```c#
T GetCachedMeta<T,>( string keyName, T defaultValue = null) 
```
Package.GetMetabut with cache.
```c#
T GetCachedMeta<T,>( string keyName, Func<T> defaultValue) 
```
Package.GetMetabut with cache.
```c#
SavedGame GetSavedGame( string name) 
```
Get a saved game by its name.
```c#
List<SavedGame> GetSavedGames( ) 
```
Get a list of metadata for all locally saved games.
## Extensions

```c#
bool IsMounted( bool downloadAndMount = false, bool withCode = false) 
```
Download and mount this package. If withCode is true we'll try to load the assembly if it exists.
```c#
Task<BaseFileSystem> MountAsync( ) 
```
Download and mount this package.PAINDAY TODO: Delete me and makeSandboxGameExtensions.MountAsynchave an optional argument
```c#
Task<BaseFileSystem> MountAsync( bool withCode) 
```
Download and mount this package. If withCode is true we'll try to load the assembly if it exists.
```c#
Task SetFavouriteAsync( bool state) 
```
Mark this package as a favourite
```c#
Task SetVoteAsync( bool up) 
```
Add your vote for this package
```c#
Task<bool> UploadFile( string absolutePath, string relativePath, Callback progress, CancellationToken token = null) 
```
Mark this package as a favourite
```c#
Task<bool> UploadFile( byte[] contents, string relativePath, Callback progress, CancellationToken token = null) 
```
Upload a file used by this package
## Nested Types

