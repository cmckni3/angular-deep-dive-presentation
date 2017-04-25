## Create a project

```sh
ng new --link-cli --routing --style scss my-project
```

```
├── e2e
├── package.json
├── protractor.conf.js
├── src
│   ├── app
│   │   ├── app-routing.module.ts
│   │   ├── app.component.ts
│   │   └── app.module.ts
│   ├── index.html
│   ├── main.ts
│   ├── polyfills.ts
│   ├── styles.scss
├── tsconfig.json
└── yarn.lock
```

Note:

Global defaults can be set using `ng set --global` or by manually editing `~/.angular-cli.json`

Example: `ng set --global defaults.styleExt=scss`