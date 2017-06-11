All I've done here is

```
create-react-app t
cd t
yarn add simple-react-form
```

and add to App.js the line

```
import { Form, Field } from "simple-react-form";
```

I get an exception on `npm start`:

```
Failed to compile.

./~/simple-react-form/src/Field.js
Module parse failed: /Users/da/personal_src/t/node_modules/simple-react-form/src/Field.js Unexpected token (173:26)
You may need an appropriate loader to handle this file type.
|     const propOptions = omit(this.props, keys(propTypes))
|     const schemaOptions = (this.getFieldSchema() && (this.getFieldSchema().srf || this.getFieldSchema().mrf)) || {}
|     const totalOptions = {...schemaOptions, ...propOptions}
|     const allowedKeys = keys({...fieldTypePropTypes, ...fieldComponent.propTypes})
|     const onlyAllowedOptions = pick(totalOptions, allowedKeys)
```

Note the link to the `src` subdirectory.

