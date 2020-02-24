# js-using
Using JavaScript

Number:
```javascript
Number('777');

const numbers = [
  (undefined + 42),     // NaN
  ('42px' - 2),         // NaN
  +"100px",             // NaN
  ('2' * '2'),          // 4
  ('42' - 40),          // 2
  (null + 2),           // 2
  parseInt('100px'),    // 100
  parseInt('12.3'),     // 12
  parseFloat('12.5em'), // 12.5
  parseFloat('12.3.4'), // 12.3
  parseInt('a123'),     // NaN
  parseInt('0xff', 16), // 255
  parseInt('ff', 16),   // 255
  parseInt('73', 36),   // 255
  Math.random(),        // 0.895984120642211
  Math.max(3, 5, -10, 0, 1), // 5
  Math.min(1, 2),  // 1
  Math.pow(2, 10), // 1024
  Math.log2(128),  // (Math.log(128) / Math.LN2) = 7
  Number('0x' + 255..toString(16)), // ff (string) -> number 255
  Number('0o' + (255).toString(8)), // 377 (string) -> number 255
  Number('0b' + 255..toString(2)),  // 11111111 (string) -> number 255
  Number(255..toString(36)),        // 73 !!!
];
```

Rounding number:
```javascript
Number(12.34.toFixed(1));// 12.3
+12.34.toFixed(5); // 12.34
0.1.toFixed(20); // 0.10000000000000000555 !!!

Math.floor(3.1); // 3
Math.floor(3.6); // 3
Math.floor(-1.1);// -2
Math.floor(-1.6);// -2

Math.ceil(3.1); // 4
Math.ceil(3.6); // 4
Math.ceil(-1.1);// -1
Math.ceil(-1.6);// -1

Math.round(3.1); // 3
Math.round(3.6); // 4
Math.round(-1.1);// -1
Math.round(-1.6);// -2

Math.trunc(3.1); // 3
Math.trunc(3.6); // 3
Math.trunc(-1.1);// -1
Math.trunc(-1.6);// -1
```

String:
```javascript
String(777);

let str = 'JavaScript'; 

str.length; // 10

str.charAt(4);      // S
str.charCodeAt(4);  // 83
str.concat(', CSS', ', CSS 3');// JavaScript, CSS, CSS 3
str.constructor("Hello");      // Hello

str.indexOf("a");     // 1
str.lastIndexOf('c'); // 5
str.match(/JavaScript/); // regexp
str.padEnd(12, '#'); // JavaScript##
str.padStart(12,'#');// ##JavaScript
str.repeat(2);// JavaScriptJavaScript

str.slice(4, 5); // S
"JS CSS".split(" ");   // ["JS", "CSS"]

str.substr(4, 6);// Script
str.substring(4,0);// Java

str.endsWith('JavaScript', 10);// true
str.includes('Jt');    // false
'Быть или не быть'.startsWith('Быть'); // true
'Быть или не быть'.startsWith('не быть'); // false
'Быть или не быть'.startsWith('не быть', 9); // true
str.search(/gg/); // -1


str.toLocaleLowerCase(); // javascript
str.toLocaleUpperCase(); // JAVASCRIPT
str.toLowerCase();       // javascript
str.toUpperCase();       // JAVASCRIPT
str.toString();          // JavaScript

" JavaScript ".trim();      // "JavaScript"
" JavaScript ".trimEnd();   // "JavaScript "
" JavaScript ".trimEnd();   // "JavaScript "
" JavaScript ".trimLeft();  // "JavaScript "
" JavaScript ".trimRight(); // " JavaScript"
" JavaScript ".trimStart(); // "JavaScript "


str.anchor("language");        // <a name="language">JavaScript</a>
str.big();                     // <big>JavaScript</big>
str.blink();                   // <blink>JavaScript</blink>
str.bold();                    // <b>JavaScript</b>
str.italics();                 // <i>JavaScript, PHP, CSS</i>
str.fixed();                   // <tt>JavaScript</tt>
str.fontcolor("#000");         // <font color="#000">JavaScript</font>
str.link('http://google.com'); // <a href="http://google.com">JavaScript, PHP, CSS</a>
str.small();                   // <small>JavaScript</small>
str.strike();                  // <strike>JavaScript</strike>
str.sub();                     // <sub>JavaScript</sub>
str.sup();                     // <sup>JavaScript</sup>

```

