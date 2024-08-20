# @aoijs/aoi.compiler

```js
const {
    sort_array,
    Compiler
} = require("@aoijs/aoi.compiler")

const mycode = `Hello, $author, your ID: $authorID`

const myfunctions = sort_array([
    "$authorID",
    "$author"
])

const compiler = new Compiler(mycode, myfunctions).start()

console.log(
    { code: compiler.get_compiled_code() },
    compiler.get_functions()
)
```
