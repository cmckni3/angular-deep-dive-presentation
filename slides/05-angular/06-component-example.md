## Components

```typescript
import { Component } from '@angular/core';

@Component({
  selector: 'home',
  styles: [`
  h1 { color: rebeccapurple; }
  `],
  template: `
  <h1>{{title}}</h1>
  `
})
export default class HomeComponent {
  public title: string = 'Hello World';
}
```

Note:

The selector is the "tag" to use inside of another component's template. It is also how the component will appear in the browser.

Components can be split into 2 categories of components, containers (smart) and presentational (dumb).