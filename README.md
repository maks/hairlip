hairlip
=======

a very tiny version of mustache

## Usage

Just pass in a data object whose direct properties will be used to substitute for tokens with matchign names in the template text.

eg.
```javascript
var hairlip = require("hairlip"),
    template = "Hi {{name}}, it is currently {{dts}}";
    data = { name: "baldrick", dts: function() { return new Date().toString()} };
console.log(hairlip(data, template));
```

*Note:* nested properties are **not** supported.

## License

BSD
