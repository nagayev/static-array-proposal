# Static array proposal

## Champion

Looking for a champion.

## Status

Stage 0, discussing the idea.

## Motivation

In system languages like C or D user can create arrays with constant size like

```c
int main(){
  int a[25];
  return 0;
}
```
Such arrays creates on the stack, not on the heap.  
These means allocation takes less time.

So I suggest add to ECMAScript object `StaticArray` with Array like API excluding possibility to change Array's size.

## Polyfills

As `StaticArray` is just Array, but located at the stack we user can use usual Array.
