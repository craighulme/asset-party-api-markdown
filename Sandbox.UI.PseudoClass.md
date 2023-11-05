# PseudoClass

## 
```c#
Derives from Enum
```

## Summary

List of CSS pseudo-classes used by the styling system for hover, active, etc.
This acts as a bit-flag.
## Fields

```c#
static PseudoClass Active = 8
```
:active- A button that is being pressed down.
```c#
static PseudoClass Empty = 128
```
:empty- Any element that has no children.
```c#
static PseudoClass FirstChild = 256
```
:first-child- The element is the first element among a group of sibling elements.
```c#
static PseudoClass Focus = 16
```
:focus- An element with input focus.
```c#
static PseudoClass Hover = 4
```
:hover- Any element with the mouse cursor hovering over it.
```c#
static PseudoClass Intro = 32
```
:intro- Present on all elements for their first frame. Useful to start CSS transitions on creation.
```c#
static PseudoClass LastChild = 512
```
:last-child- The element is the last element among a group of sibling elements.
```c#
static PseudoClass None = 0
```
No pseudo-class.
```c#
static PseudoClass OnlyChild = 1024
```
:only-child- The element is the only child of their parent element.
```c#
static PseudoClass Outro = 64
```
:outro- The element has been marked for deletion, and will be deleted once all CSS transitions on it has stopped.Transitions can be started here to gracefully remove the element visually.
```c#
static PseudoClass Unknown = 2
```
Unused.
## Referencing Members

```c#
PseudoClass = StyleSelector.Flags
```
```c#
abstract PseudoClass = IPanel.PseudoClass { get; set; } 
```
```c#
virtual PseudoClass = Panel.PseudoClass { get; set; } 
```
```c#
bool = Panel.Switch( PseudoClass, bool ) 
```
