# DisplayInfo

## ```c#
Derives from ValueType
```

## Summary

Collects all the relevant info (such as description, name, icon, etc) from attributes and other sources about a type or type member.
## Fields

```c#
string[] Alias
```
Possible aliases for this type or member, if any. (AliasAttribute)
```c#
bool Browsable
```
Whether this member should be visible in a properties sheet (HideInEditorAttribute)
```c#
string ClassName
```
"Internal" class name of this type or member. This typically should be all lowercase and without weird symbols or whitespace.
```c#
string Description
```
The summary or description of this type or member.
```c#
string Fullname
```
Namespace.ParentClass.Class.Member
```c#
string Group
```
Group or category of this type or member. (CategoryAttribute)
```c#
string Icon
```
Material icon of this type or member. (IconAttribute)
```c#
string Name
```
The name of this type or member.
```c#
string Namespace
```
Namespace of this type
```c#
int Order
```
Order of this member for UI ordering purposes. (OrderAttribute)
```c#
string Placeholder
```
Placeholder text for string type properties. (PlaceholderAttribute)
Placeholder text is displayed in UI when input text field is empty.
```c#
string[] Tags
```
Tags of this type or member. (TagAttribute)
## Methods

```c#
static DisplayInfo For( object t, bool inherit = true) 
```
Retrieves display info about a given objects type.
```c#
static DisplayInfo[] ForEnumValues( Type t) 
```
Returns display info for each member of an enumeration type.
```c#
static ValueTuple[] ForEnumValues<T,>( ) 
```
Returns display info for each member of an enumeration type.
```c#
static DisplayInfo ForMember( MemberInfo t, bool inherit = true) 
```
Retrieves display info about a given member or type.
```c#
static DisplayInfo ForType( Type t, bool inherit = true) 
```
Retrieves display info about a given type.
```c#
bool HasTag( string t) 
```
Returns whether this type or member has given tag. (TagAttribute)
## Referencing Members

```c#
Option = NavigationView.AddPage( DisplayInfo, Widget ) 
```
```c#
DisplayInfo = EntityEntry.DisplayInfo
```
```c#
DisplayInfo = NodeUI.DisplayInfo { get; set; } 
```
```c#
DisplayInfo = MemberDescription.GetDisplayInfo( ) 
```
```c#
protected DisplayInfo? = PropertyEditorWidget.PropertyDisplay { get; set; } 
```
```c#
void PropertyRow.SetLabel( DisplayInfo ) 
```
```c#
virtual void PropertyEditorWidget.SetPropertyDisplayInfo( DisplayInfo ) 
```
