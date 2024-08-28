<h1 align="center">
    Validator
</h1>

<p align="center">
     <i>A 🔋-included, supercharged & customizable,<br>string validation library for Arturo</i> 
     <br><br>
     <img src="https://img.shields.io/github/license/arturo-lang/grafito?style=for-the-badge">
    <img src="https://img.shields.io/badge/language-Arturo-orange.svg?style=for-the-badge">
</p>


--- 
 
<!--ts-->

* [What does this package do?](#what-does-this-package-do)
* [How do I use it?](#how-do-i-use-it)
* [Function Reference](#function-reference)
* [License](#license)   

<!--te-->
 
---

### What does this package do?

This package provides a function (`valid?`) that allows to check and validate strings, based on different built-in schemes/patterns, e.g e-mails, urls, etc.

### How do I use it?

Simply `import` it and use the included `valid?` function:

```red
import "validator"!

valid?.url "https://arturo-lang.io"
; => true

valid?.email "loremIpsum@
; => false
```

And we may also check more than one strings:

```red
valid?.email ["my@email.com", "info@google.com"]
; => true
```

> [!TIP]
> Different type of checks may accept different extra params, so you'd better have a look into the reference first! 😉


### Function reference

#### `valid?`

##### Description

check if given string is valid

##### Usage

<pre>
<b>valid?</b> <ins>str</ins> <i>:string :block</i>
</pre>

##### Attributes

| Option | Description |
|----|----|
| email | verify e-mail address | 
| url | verify URL |

##### Returns

- *:logical*

<hr/>

### License

MIT License

Copyright (c) 2024 Yanis Zafirópulos

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
