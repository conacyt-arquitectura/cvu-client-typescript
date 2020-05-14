# Cliente de CVU en TypeScript

El cliente para TypeScript del microservicio de CVU de CONACYT.

# Instalación

`npm i @conacyt/cvu-client`

# Uso

Para usar en un archivo TypeScript:

```ts
import { CvuApi } from "cvu-client";

const cvuApi = new CvuApi({}, 'http://localhost:8081');
cvuApi
  .getPersonaFisicaByCvu("1234")
  .then(res => console.log(res.data));
  .catch(console.error);
```

Para usar en un archivo JavaScript:

```js
const CvuApi = require("cvu-client").CvuApi;

const cvuApi = new CvuApi({}, 'http://localhost:8081');
cvuApi
  .getPersonaFisicaByCvu("1234")
  .then(res => console.log(res.data));
  .catch(console.error);
```
