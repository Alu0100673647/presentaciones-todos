# 9. Import

Esta nueva palabra clave forma parte del estándar, pero aún no ha sido implenetado por V8 de forma nativa.

Import funciona en definitiva como un `require`, pero a bajo nivel cambia mucho respecto a `commonjs`.

## Importar una variable

Antes usábamos `require` para importar una variable:

```JavaScript
const _ = require('lodash')

let aux1 = _.tail([1, 2, 3])
let aux2 = _.concat([1, 2], [3, 4])

console.log(aux1)
console.log(aux2)
```

Pero ahora con `import` tenemos una sintaxis más clara:

```JavaScript
import _ from 'lodash'

let aux1 = _.tail([1, 2, 3])
let aux2 = _.concat([1, 2], [3, 4])

console.log(aux1)
console.log(aux2)
```

Incluso, podemos combinarlo con el uso de las deconstrucciones:

```JavaScript
import { tail, concat } from 'lodash'

let aux1 = tail([1, 2, 3])
let aux2 = concat([1, 2], [3, 4])

console.log(aux1)
console.log(aux2)
```
