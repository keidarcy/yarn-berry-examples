# nm-linker-pnpm

### `.yarnrc.yml`

```yml
# ...
nodeLinker: pnpm
# ...
```

### features

- no `.pnp.cjs`
- `node_modules` exists.
- `pnpm` similar symlink structure.
- no [phantom](https://rushjs.io/pages/advanced/phantom_deps/) or [doppelgangers](https://rushjs.io/pages/advanced/npm_doppelgangers/)

### node_modules content

```
╰─❯ tree -a node_modules
node_modules
├── .store
│  └── lodash.chunk-npm-4.2.0-a54ef4d7dd
│     └── node_modules
└── lodash.chunk -> .store/lodash.chunk-npm-4.2.0-a54ef4d7dd/node_modules/lodash.chunk
```

### execution

```
node index.js
```
