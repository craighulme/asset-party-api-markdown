# SpeechRecognition

## 
```c#
Derives from object
```

## Summary

Whether or not we are currently listening for speech.
## Properties

```c#
static bool IsListening { get; } 
```
Whether or not we are currently listening for speech.
```c#
static bool IsSupported { get; } 
```
Whether or not speech recognition is supported and a language is available.
## Methods

```c#
static bool Listen( OnSpeechRecognized callback, string[] choices = null) 
```
No Summary
```c#
static void Start( OnSpeechResult callback, IEnumerable<string> choices = null) 
```
Start listening for speech to recognize as text. When speech has been recognized the callback
will be invoked, the callback will also be invoked if recognition fails.
```c#
static void Stop( ) 
```
Stop any active listening for speech.
## Nested Types

