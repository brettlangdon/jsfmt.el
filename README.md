jsfmt.el
========

emacs plugin to allow running [jsfmt](https://rdio.github.io/jsfmt) on javascript files.

this is basically a clone of the necessary code from `go-mode` for running `gofmt` but used `jsfmt` instead.

## Installing

Install [jsfmt](https://rdio.github.io/jsfmt):

```bash
npm install -g jsfmt
```

Download and place `jsfmt.el` in `~/.emacs.d`

Modify your `~/.emacs` file to include:
```lisp
(load "~/.emacs.d/jsfmt")
```

Add the following to `~/.emacs` to run `jsfmt` before saving file:
```lisp
(add-hook 'before-save-hook 'jsfmt-before-save)
```

## License
The MIT License (MIT) Copyright (c) 2014 Brett Langdon <brett@blangdon.com> (http://brett.is)

Permission is hereby granted, free of charge, to any person obtaining a copy of this softwareand associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
