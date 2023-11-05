# CircularBuffer<T>

## 
```c#
Implements IEnumerable<T>
```

## Summary

Circular buffer, push pop and index access is always O(1).
## Type Parameters

```c#
T
```
No Summary
## Constructors

```c#
CircularBuffer( int capacity) 
```
Initializes a new instance of theUtility.CircularBuffer<T>class.
```c#
CircularBuffer( int capacity, T[] items) 
```
Initializes a new instance of theUtility.CircularBuffer<T>class.
## Properties

```c#
int Capacity { get; } 
```
Maximum capacity of the buffer. Elements pushed into the buffer after
maximum capacity is reached (IsFull = true), will remove an element.
```c#
bool IsEmpty { get; } 
```
True if has no elements.
```c#
bool IsFull { get; } 
```
Boolean indicating if Circular is at full capacity.
Adding more elements when the buffer is full will
cause elements to be removed from the other end
of the buffer.
```c#
int Size { get; } 
```
Current buffer size (the number of elements that the buffer has).
## Methods

```c#
virtual IEnumerator<T> GetEnumerator( ) 
```
ImplementsIEnumerable`1.GetEnumeratorReturns an enumerator that iterates through this buffer.
```c#
T Back( ) 
```
Element at the back of the buffer - this[Size - 1].
```c#
void Clear( ) 
```
Clears the contents of the array. Size = 0, Capacity is unchanged.
```c#
T Front( ) 
```
Element at the front of the buffer - this[0].
```c#
void PopBack( ) 
```
Removes the element at the back of the buffer. Decreasing the
Buffer size by 1.
```c#
void PopFront( ) 
```
Removes the element at the front of the buffer. Decreasing the
Buffer size by 1.
```c#
void PushBack( T item) 
```
Pushes a new element to the back of the buffer. Back()/this[Size-1]
will now return this element.When the buffer is full, the element at Front()/this[0] will be
popped to allow for this new element to fit.
```c#
void PushFront( T item) 
```
Pushes a new element to the front of the buffer. Front()/this[0]
will now return this element.When the buffer is full, the element at Back()/this[Size-1] will be
popped to allow for this new element to fit.
```c#
T[] ToArray( ) 
```
Copies the buffer contents to an array, according to the logical
contents of the buffer (i.e. independent of the internal
order/contents)
```c#
IList<ArraySegment<T>> ToArraySegments( ) 
```
Get the contents of the buffer as 2 ArraySegments.
Respects the logical contents of the buffer, where
each segment and items in each segment are ordered
according to insertion.Fast: does not copy the array elements.
Useful for methods likeSend(IList<ArraySegment<Byte>>).Segments may be empty.
## Operators

```c#
T this[ int index, ] 
```
Index access to elements in buffer.
Index does not loop around like when adding elements,
valid interval is [0;Size[
