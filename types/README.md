# Types

Все типы: number, bigint, boolean, string, undefined, null, object, symbol

Number:
```javascript
const INFINITY_1 = 1 / 0;
const INFINITY_2 = 1e500;

const numbers = [
  typeof 0,
  typeof 3.14,
  typeof 1e3,  // 1 * 1000 = 1000
  typeof 1e-3, // 1 / 1000 = 0.001
  typeof 0xff, // шестнадцатеричная форма 255
  typeof 0xFF, // шестнадцатеричная форма 255
  typeof 0b11111111, // бинарная форма 255
  typeof 0o377, // восьмеричная форма 255
  typeof INFINITY_1, // специальное значение бесконечность
  typeof INFINITY_2, // специальное значение бесконечность
  typeof NaN,
];
```
Bigint:
```javascript
const bigint = [
  typeof BigInt(10),
  typeof BigInt("1234567890123456789012345678901234567890"),
  typeof 1234567890123456789012345678901234567890n,
];
```
boolean:
```javascript
const boolean = [
  typeof true,
  typeof false,
  typeof (0.1 + 0.2 == 0.3),      // false
  typeof (0 === -0),              // true
  typeof isNaN(NaN),              // true
  typeof isNaN("str"),            // true
  typeof (NaN === NaN),           // false
  typeof isFinite("15"),          // true
  typeof isFinite("str"),         // false
  typeof isFinite(Infinity),      // false
  typeof Object.is(NaN, NaN),     // true
  typeof Object.is(+"100px", NaN),// true
  typeof Object.is(0, -0),        // false
  typeof Boolean(''),             // false
  typeof Boolean(' '),            // true
  typeof Boolean('JavaScript'),   // true
  typeof Boolean('0'),            // true
  typeof Boolean(0),              // false
  typeof Boolean(null),           // false
  typeof Boolean([]),             // true
  typeof Boolean({}),             // true
  typeof Boolean(function(){}),   // true
  typeof (2 == '2'),              // true
  typeof (2 === '2'),             // false
  typeof (undefined == null),     // true
  typeof (undefined === null),    // false
  typeof ('0' == false),          // true
  typeof ('0' == 0),              // true
  typeof (0 == 0),                // true
  typeof (false == ''),           // true
  typeof (false == []),           // true
  typeof (false == {}),           // false
  typeof ('' == 0),               // true
  typeof ('' == []),              // true
  typeof ('' == {}),              // false
  typeof (0 == []),               // true
  typeof (0 == []),               // true
  typeof (0 == {}),               // false
  typeof (0 == null),             // false
];
```
string:
```javascript
const string = [
  typeof 'JavaScript',
  typeof "JavaScript",
  typeof `JavaScript`,
  12.34.toFixed(5), // 12.34000
];
```
object:
```javascript
const object = [
  typeof Object.create({}),
  typeof {},
  typeof function() {},
  typeof null,
];
```
Symbol:
```javascript
const symbol = [
  typeof Symbol('JavaScript'),
];
```

Undefined:
```javascript
let noVariable;

const symbol = [
  typeof noVariable, // undefined
  typeof undefined,
];
```
