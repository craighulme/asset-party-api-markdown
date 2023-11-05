# PackageUsageStats

## Derives from ValueType

## Summary

Statistics for user interactions with this package
## Properties

```c#
long[] DailySeconds { get; set; } 
```
A historic array of number of seconds played. Last entry is yesterday.
```c#
long[] DailyUsers { get; set; } 
```
A historic array of daily unique users. Last entry is yesterday.
```c#
Group Day { get; set; } 
```
Usage for the last 24 hours
```c#
Group Month { get; set; } 
```
Usage for the last 3 days
```c#
Group Total { get; set; } 
```
Total lifetime usage stats
```c#
double Trend { get; set; } 
```
The trend is a number that represents whether it's been popular recently. Higher means more popular.
```c#
long UsersNow { get; set; } 
```
How many users are using it right now
```c#
Group Week { get; set; } 
```
Usage for the last week
## Nested Types

## Referencing Members

```c#
PackageUsageStats = Package.Usage { get; set; } 
```
