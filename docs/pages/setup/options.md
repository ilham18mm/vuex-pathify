# Options

> Configure Pathify's options

#### `mapping`

- Type: String | Function
- Default: "standard"

The **mapping** option helps determine how Pathify should map Pathify operations to Vuex store members.

You can choose from a couple of common presets, or provide a custom function.

See the [mapping](/setup/mapping.md) page for more details.

#### `deep`

- Type: Boolean
- Default: true

The **deep** option premits sub-property read and writes for store members of the `Object` type:

```js
store.set('sort@order', 'asc')
```

Setting deep to `false` will cause sub-property access to fail and will generate a console error in development if sub-property access is attempted.


#### `strict`

> Not implemented yet

- Type: Boolean
- Default: true

The **strict** option causes an error to be thrown if attempting to access to properties that don't exist.



#### `cache`

> Not implemented yet

- Type: Boolean
- Default: true

The **cache** option enables caching of mapping results, making for speedier lookups when paths are accessed or computed properties are recreated.

Disabling caching has a negligible performance impact.
