# nm-linker-pnp

### `.yarnrc.yml`

```yml
# ...
nodeLinker: pnp
# ...
```

### features

- `.pnp.cjs` exists.
- no `node_modules`.
- gitignore do not ignore `.yarn/cache`, commit it
- `yarn.lock`

```
"zero-install@workspace:.":
  version: 0.0.0-use.local
  resolution: "zero-install@workspace:."
  dependencies:
    lodash.chunk: ^4.2.0
  languageName: unknown
  linkType: soft
```

### execution

```
yarn node index.js
```
