## Container component Example

```typescript
@Component({
    selector: 'app',
    template: `<h3>Party Planner</h3>
      <person-input
        (addPerson)="addPerson($event)"
      >
      </person-input>`
})
export class App {
    public people;
    addPerson(name) {
      this.people.push({id: id(), name});
    }
}
```