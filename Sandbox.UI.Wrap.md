# Wrap

## Derives from Enum

## Summary

Possible values forflex-wrapCSS property.
## Fields

```c#
static Wrap NoWrap = 0
```
Elements will be laid out in a single line.
```c#
static Wrap Wrap = 1
```
Elements will be moved to subsequent lines on overflow.
```c#
static Wrap WrapReverse = 2
```
Same asWrap.Wrap, but the line order will be reversed, i.e. if one item overflows the width,
it will be placed on the first line, and the others will be placed on the second line.
## Referencing Members

```c#
Wrap? = BaseStyles.FlexWrap { get; set; } 
```
