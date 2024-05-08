# js-yaml + cloudformation-schema

Based on [@serverless/utils/cloudformation-schema][cloudformation-schema], this package provides a YAML schema for js-yaml library that includes AWS Cloudformation specific short-hand syntaxes (i.e. !Ref or !GetAtt).

```js
const yaml = require('js-yaml');
const fs   = require('fs');
const cloudFormationSchema = require('@inetsys/js-yaml-cloudformation-schema');

yaml.load(fs.readFileSync('serverless.yml', { schema: cloudFormationSchema });
```


[cloudformation-schema]: https://github.com/serverless/utils/blob/main/cloudformation-schema.js
