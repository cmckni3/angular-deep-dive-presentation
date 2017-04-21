## Module Example

```typescript
import { NgModule, CommonModule } from '@angular/core';
import { HomeComponent } from './home.component';
import { HomeService } from './home.service';
export default class HomeModule {
  declarations: [
    HomeComponent
  ],
  imports: [CommonModule],
  exports: [HomeComponent],
  providers: [HomeService]
}
```