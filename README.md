# sic-db
A small javascript (hash) database of sic codes and helper functions

### Usage

Use npm to install in your project:
```sh
npm install sic-db
```
or, clone and include in your project using require (CommonJS, NodeJS):
```javascript
var sicdb = require('sic-db');
```

or, simply include as a script tag:
```html
<script src="sicdb.js" />
```

It exposes a few hash objects such as:

- sicdb.divs which provides full division names as values corresponding to the division code ("A" - "K")

- sicdb.divs_cats which provides relation from division codes to major (2 digit) category code using division code as key ("A" - "K") and associated values stored as an array

- sicdb.list which provides the complete hash of sic major category (2 digit), sub-category (3 digit) and SIC (4 digit) codes stored as keys with category names stored as corresponding values.

- sicdb.cats_divs which provides a reverse index of sicdb.divs_cats such that major category (2 digit) codes are the keys and their associated values represent sicdb.divs entries (keys).

TODO: provide some commonly used helper functions, also unit-testing and coverage

Contributions are welcome
