# Primate Data Domains

Domains add a layer of persistance to Primate. They are backed by data stores 
with the default being a transient in-memory store. Additional stores exist for
filesystem (flat), JSON, and MongoDb.

## Fields

A record in the domain's store is described using the static `fields` property.

```js
// fields.js
```

### Short notation

Field types may be any constructible JavaScript object, including other
domains. When using other domains as types, data integrity (on saving) is
ensured.

```js
// short-notation.js
```

### Predicates

Field types may also be specified as an array, to specify additional predicates
aside from the type.

```js
// predicates.js
```

## Stores

Stores interface data. Primate comes with volatile in-memory store used as a
default. Other stores can be imported as modules.

All stores are loaded from `stores`.

## License

MIT
