---
hide_title: true
custom_edit_url: null
pagination_prev: null
pagination_next: null
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@rushstack/node-core-library](./node-core-library.md) &gt; [Sort](./node-core-library.sort.md) &gt; [sortBy](./node-core-library.sort.sortby.md)

## Sort.sortBy() method

Sorts the array according to a key which is obtained from the array elements. The result is guaranteed to be a stable sort.

<b>Signature:</b>

```typescript
static sortBy<T>(array: T[], keySelector: (element: T) => any, comparer?: (x: any, y: any) => number): void;
```

## Parameters

| Parameter   | Type                          | Description |
| ----------- | ----------------------------- | ----------- |
| array       | T\[\]                         |             |
| keySelector | (element: T) =&gt; any        |             |
| comparer    | (x: any, y: any) =&gt; number |             |

<b>Returns:</b>

void

## Example

```ts
let array: string[] = ['aaa', 'bb', 'c'];
Sort.sortBy(array, (x) => x.length); // [ 'c', 'bb', 'aaa' ]
```