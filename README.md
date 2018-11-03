# laravel-mix-rest-spread-issue

## Symptom

Rest spread operator fails to parse when importing src from node module.

The operator is properly complied though when used in the local source (see `works` branch - _note the copied source from node module_).

```
Module parse failed: Unexpected token (271:8)
You may need an appropriate loader to handle this file type.
|     _getConfig(config) {
|       config = {
|         ...Default,
|         ...config
|       }
 @ ./src/index.js 1:0-35
 @ multi ./src/index.js
```

## Steps to Reproduce

- `yarn`
- `yarn dev`
