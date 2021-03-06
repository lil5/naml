
[![](https://raw.githubusercontent.com/MarkTiedemann/naml/master/logo.png)](https://github.com/MarkTiedemann/naml)

--------

[![](https://travis-ci.org/MarkTiedemann/naml.svg?branch=master)](https://travis-ci.org/MarkTiedemann/naml)
[![](https://david-dm.org/MarkTiedemann/naml.svg)](https://david-dm.org/MarkTiedemann/naml) [![](https://img.shields.io/node/v/naml.svg)](https://www.npmjs.com/package/naml)

- **Simple, unified API.**
- **Freely convert between:**
<br><br>
  - **JSON** (JavaScript Object Notation): `.json`
  - **HJSON** (Human JSON): `.hjson`
  - **JSON5** (ES5 JSON): `.json5`
  - **CSON** (CoffeeScript Object Notation): `.cson`
  - **YAML** (Yet Another Markup Language): `.yaml`
  - **TOML** (Tom's Obvious, Minimal Language): `.toml`
  - **INI** (Initialization File Format): `.ini`

## Installation

```sh
npm install naml
```

## CLI

```sh
naml [input-file] [output-file]
```
**Example:** `naml path/to/input.yaml path/to/output.json`

## API

```js
const NAML = require('naml')
```

### `NAML.parse(string, type)`

- **string** `{String}`: the String to be parsed
- **type** `{String}`: the input type; one of the following: `json`, `hjson`, `json5`, `cson`, `yaml`, `toml`, `ini` (may be prefixed with a `.`)
- **returns** `{Object}`: the resulting Object
- **throws** `{Error}`: if parsing failed

### `NAML.stringify(object, type)`

- **object** `{Object}`: the Object to be stringified
- **type** `{String}`: the input type; one of the following: `json`, `hjson`, `json5`, `cson`, `yaml`, `toml`, `ini` (may be prefixed with a `.`)
- **returns** `{String}`: the resulting String
- **throws** `{Error}`: if stringifying failed

## License

[WTFPL](http://www.wtfpl.net/) – Do What the F*ck You Want to Public License.

Made with :heart: by [@MarkTiedemann](https://twitter.com/MarkTiedemannDE).
