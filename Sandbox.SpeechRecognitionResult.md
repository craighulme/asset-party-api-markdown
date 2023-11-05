# SpeechRecognitionResult

## 
```c#
Derives from ValueType
```

## Summary

A result from speech recognition.
## Properties

```c#
float Confidence { get; init; } 
```
From 0-1 how confident are we that this is the correct result?
```c#
bool Success { get; init; } 
```
Did we successfully find a match?
```c#
string Text { get; init; } 
```
The text result from speech recognition.
## Referencing Members

```c#
virtual IAsyncResult = OnSpeechResult.BeginInvoke( SpeechRecognitionResult, AsyncCallback, object ) 
```
```c#
virtual void OnSpeechResult.Invoke( SpeechRecognitionResult ) 
```
