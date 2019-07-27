# ofxARToolKitPlus

## Introduction
original ofxAddons from 
https://github.com/karldd/ofxARToolkitPlus

refactory repo</br>

## Licence
The code in this repository is available under the [MIT License](https://secure.wikimedia.org/wikipedia/en/wiki/Mit_license).

Copyright (c) [17/12/2012] [James Kong]

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## Installation


## Dependencies
- ofxOpenCV

## Compatibility


## Known issues
currently, linux 64 / win64 VS2019 only tested. </br>

clone https://github.com/paroj/artoolkitplus repo, compile `static` library as written below.

| for your costum compilation, build the static library rather that shared library.
|
| in CMakeLists.txt line 32
| comment 
```
    #add_library(ARToolKitPlus SHARED ${HEADERS_AR} ${SOURCES_AR})
```
| replace with
```
	add_library(ARToolKitPlus STATIC ${HEADERS_AR} ${SOURCES_AR})
```

## Version history

### Version 0.1 (2013-01-30):

and open source library from
https://launchpad.net/artoolkitplus

- deprecated codeblock example
+ xcode example from 
[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/fishkingsin/ofxartoolkitplus/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

### Version 0.2 (2019-07-27):
- fix for modern OF standard 
	- testApp -> ofApp
	- fix deprecated OF functions.
- linux64 static library(.a) updated and tested.
- win64 (vs) static library updated and tested with vs2019.