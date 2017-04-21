## Structural Directive Example

```html
<ul>
  <li *ngFor="let person of people">{{person.name}}</li>
</ul>
```

Note:

The example shows the use of `ngFor` to generate an element, `li`, for each person's name.