# ObservableDictionary<TKey,TValue>

## Derives from object
Implements IDictionary<TKey, TValue>, INotifyCollectionChanged, INotifyPropertyChanged

## Summary

A dictionary with callbacks for when changes occur.
## Type Parameters

```c#
TKey
```
No Summary
```c#
TValue
```
No Summary
## Constructors

```c#
ObservableDictionary( ) 
```
No Summary
```c#
ObservableDictionary( IDictionary<TKey, TValue> dictionary) 
```
No Summary
```c#
ObservableDictionary( IEqualityComparer<TKey> comparer) 
```
No Summary
```c#
ObservableDictionary( int capacity) 
```
No Summary
```c#
ObservableDictionary( IDictionary<TKey, TValue> dictionary, IEqualityComparer<TKey> comparer) 
```
No Summary
```c#
ObservableDictionary( int capacity, IEqualityComparer<TKey> comparer) 
```
No Summary
## Properties

```c#
virtual int Count { get; } 
```
ImplementsICollection`1.Count
```c#
virtual bool IsReadOnly { get; } 
```
ImplementsICollection`1.IsReadOnly
```c#
virtual ICollection<TKey> Keys { get; } 
```
ImplementsIDictionary`2.Keys
```c#
virtual ICollection<TValue> Values { get; } 
```
ImplementsIDictionary`2.Values
```c#
protected IDictionary<TKey, TValue> Dictionary { get; } 
```
The dictionary being observed.
## Methods

```c#
virtual void Add( TKey key, TValue value) 
```
ImplementsIDictionary`2.Add
```c#
virtual void Add( KeyValuePair<TKey, TValue> item) 
```
ImplementsICollection`1.Add
```c#
virtual void Clear( ) 
```
ImplementsICollection`1.Clear
```c#
virtual bool Contains( KeyValuePair<TKey, TValue> item) 
```
ImplementsICollection`1.Contains
```c#
virtual bool ContainsKey( TKey key) 
```
ImplementsIDictionary`2.ContainsKey
```c#
virtual void CopyTo( KeyValuePair[] array, int arrayIndex) 
```
ImplementsICollection`1.CopyTo
```c#
virtual IEnumerator<KeyValuePair<TKey, TValue>> GetEnumerator( ) 
```
ImplementsIEnumerable`1.GetEnumerator
```c#
protected virtual void OnPropertyChanged( string propertyName) 
```
Called when a property (such as element count) of the dictionary has changed.
```c#
virtual bool Remove( TKey key) 
```
ImplementsIDictionary`2.Remove
```c#
virtual bool Remove( KeyValuePair<TKey, TValue> item) 
```
ImplementsICollection`1.Remove
```c#
virtual bool TryGetValue( TKey key, out TValue value) 
```
ImplementsIDictionary`2.TryGetValue
```c#
void AddRange( IDictionary<TKey, TValue> items) 
```
Merge given dictionary into this one.
## Events

```c#
CollectionChanged( object sender, NotifyCollectionChangedEventArgs e) 
```
Called when the dictionary's key-value pairs have changed.
```c#
PropertyChanged( object sender, PropertyChangedEventArgs e) 
```
Called when a property (such as element count) of the dictionary has changed.
## Operators

```c#
TValue this[ TKey key, ] 
```
ImplementsIDictionary`2.Item
