---
"pacquet": patch
---

pnpm now writes each command shim in a `node_modules/.bin` directory it just created without first reading a path it knows holds nothing. A warm install of a 76 project workspace makes about 1,500 fewer filesystem calls [#14540](https://github.com/pnpm/pnpm/issues/14540).
