## RxJS Example

```typescript
const source = Rx.Observable.timer(200, 100)
    .take(3);

const subscription = source.subscribe(
    function (x) {
        console.log('Next: ' + x);
    },
    function (err) {
        console.log('Error: ' + err);   
    },
    function () {
        console.log('Completed');   
    });

// => Next: 200
// => Next: 100
// => Next: 100
// => Completed
```

Note:

The example shows a timer that produces an initial value after 200ms. Subsequent events are produced every 100ms.

This example shows automatically unsubscribing