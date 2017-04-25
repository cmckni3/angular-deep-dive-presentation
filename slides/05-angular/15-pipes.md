## Pipes

> An Angular pipe is a function that transforms input values to output values for display in a view.

```typescript
...

@Component({
  selector: 'my-component',
  template: `
  <!-- Today is Apr 21, 2017 -->
  <span>Today is {{ currentDate | date }}</span>
  `
})
export class MyComponent {
  public currentDate = new Date();
}
```

Note:

- Pipes can be thought of as formatters
- Custom formatters can provide powerful functionality

The example represents formatting a date string or Date object as a string in the view
