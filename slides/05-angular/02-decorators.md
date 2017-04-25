## Decorator example

```typescript
import { deprecate } from 'core-decorators';
import { compact } from 'lodash';

class Person {
  ...
  // deprecate the name method using a decorator
  @deprecate('Use the fullName method instead')
  get name() {
    return compact([this.first_name, this.last_name]).join(' ');
  }

  get fullName() {
    ...
  }
}
```