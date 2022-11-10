# nm-linker-node-modules

### `.yarnrc.yml`

```yml
yarnPath: ".yarn/releases/yarn-berry.cjs"
nodeLinker: node-modules
```

### features

- no `.pnp.cjs`
- `node_modules` exists.
- `.yarn/cache` only used for installation.

####  recommend settings

```yml
enableGlobalCache: true # move zip files from cacheFolder to global folder like $HOME/
# cacheFolder: "./.yarn/cache"
compressionLevel: 0
```

### node_modules content

```
node_modules
├── .yarn-state.yml
└── lodash.chunk
   ├── index.js
   ├── LICENSE
   ├── package.json
   └── README.md
```

### execution

```
node index.js
```
