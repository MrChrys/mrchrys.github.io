# ***MrDB***
## MrDB is a module made to save your variables in local db

### [[BETA] Docs](https://mrchrys.github.io/mrdb/docs)

# ***Instalation***
```
npm i mrdb
```

## **<span style="color:lime">Pros</span>**
#### Save your variables in a json using functions or even manually
#### MrDB is a DB module that has no dependents

## **<span style="color:red">Cons</span>**
#### Easily hackable
#### Everything must have bugs, even real life has!
<br>

# ***<span style="color:#c28e00">Usage</span>***
## Set variable
```js
const db = require("mrdb")

console.log(db.get("")) // expected output: {}
db.set("string", "I am a string!")
console.log(db.get("")) // expected output: {string: 'I am a string!'}
```

## Set a property into a object variable
```js
const db = require("mrdb")

console.log(db.get("")) // expected output: {}
db.set("obj", {})
console.log(db.get("")) // expected output: {obj: {}}
db.set("obj.code", "MRDB-UBBO-THGX")
console.log(db.get("")) // expected output: {obj: {code: "MRDB-UBBO-THGX"}}
```

## Delete variable or property
```js
const db = require("mrdb")

db.set("obj", {a:2})
console.log(db.get("")) // Expected output: { obj: { a: 2 } }
db.delete("obj.a")
console.log(db.get("")) // Expected output: { obj: {}}
db.delete("obj")
console.log(db.get("")) // Expected output: {}
```
