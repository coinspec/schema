# Opencrypto Schema v1-draft

Schemas for structured cryptocurrency-related data in [JSON Schema](http://json-schema.org/) standart.

## Structure

* Models
  * **[Asset](/models/asset.json)** ([example](/examples/models/asset.json))
  * **[Exchange](/models/exchange.json)** ([example](/examples/models/exchange.json))
  * **[Wallet](/models/wallet.json)** ([example](/examples/models/wallet.json))
  * **[Tracker](/models/tracker.json)** ([example](/examples/models/tracker.json))

## Usage

### Hosted version (standalone)
You can use web `schema.opencrypto.io` for fetching schemas, format:
```
https://schema.opencrypto.io/<file>
```

For example:
* https://schema.opencrypto.io/models/asset.json
* https://schema.opencrypto.io/examples/models/asset.json
* ...

### Locally as Node.js or CommonJS module
Install it via `npm`:
```bash
npm install opencrypto-schema
```

And use it inside your script:
```js
var Schema = require('opencrypto-schema')

// now you can access schemas by dot notation:
var assetSchema = Schema.models.asset

// or you can do it more simpler:
var schemaModels = require('opencrypto-schema').models

// or if you want only one specific schema:
var assetSchema = require('opencrypto/models/asset')
```

## Licence
MIT
