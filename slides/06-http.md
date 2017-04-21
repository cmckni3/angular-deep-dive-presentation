## Angular HTTP Service

> Http is available as an injectable class, with methods to perform http requests

```typescript
import { Injectable } from '@angular/core';
import { Http, Response } from '@angular/http';
import { Observable } from 'rxjs/Observable';
import 'rxjs/add/operator/catch';
import 'rxjs/add/operator/map';
import { Hero } from './hero';
@Injectable()
export class HeroService {
  private heroesUrl = 'api/heroes';  // URL to web API
  constructor (private http: Http) {}
  getHeroes(): Observable<Hero[]> {
    return this.http.get(this.heroesUrl)
                    .map((res: Response) => res.json())
                    .catch(() => {
                      // Handle errors here
                    });
  }
}
```