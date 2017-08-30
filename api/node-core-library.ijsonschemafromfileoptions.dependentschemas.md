<!-- docId=node-core-library.ijsonschemafromfileoptions.dependentschemas -->

[Home](./index.md) &gt; [node-core-library](./node-core-library.md) &gt; [IJsonSchemaFromFileOptions](./node-core-library.ijsonschemafromfileoptions.md)

# IJsonSchemaFromFileOptions.dependentSchemas property

Other schemas that this schema references, e.g. via the "$ref" directive.

**Signature:**
```javascript
dependentSchemas: JsonSchema[]
```

## Remarks

The tree of dependent schemas may reference the same schema more than once. However, if the same schema "id" is used by two different JsonSchema instances, an error will be reported. This means you cannot load the same filename twice and use them both together, and you cannot have diamond dependencies on different versions of the same schema. Although technically this would be possible to support, it normally indicates an error or design problem. JsonSchema also does not allow circular references between schema dependencies.