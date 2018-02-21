# Package Change String
Change/Replace the characters of a string. 

## Instal
In bash

```bash
npm install semver
```
```bash
npm install repeat-string
```

## Use

#### Arrays
Value is a string, wich will be replaced by grawlix.

```js
/* `butt` > `@#$%` */
function grawlix(value, pattern) {
  var chars = pattern || grawlixPattern;
  var length = typeof value === 'number' ? value : value.length;
  var count = chars.length;
  return repeat(chars, floor(length / count)) + chars.slice(0, length % count);
}
```


## License
MIT license

