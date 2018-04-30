# Babel every things
Babel is a tool to transpiling (compiling) ES6/ES7 to ES5
* Babel doesn't do anything. It uses presets for compiling the code
## babel-cli
babel-cli is tool that used for transpiling the code through the command line
* Install babel-cli globally
```
npm install babel-cli -g
```
* Install babel-cli locally
```
npm install babel-cli --save-dev
```
### Babel's advantages:
* Different projects on same machine can use different version of Babel
* Is independent with dev environment

Use babel to compile a javascript file from ES6 to ES5
```
babel example.js --out-file example.compiled.js
```
* *--out-file* : option for compiling a file, we can use *--out-dir* for compiling all files inside a directory

### Babel to transiple a directory
```
babel ./src -d ./build -w
```
Option *-w* was used to watch changes on **src** folder. Babel will transpile the code and save results into build folder

## babel-register

**This module is not recommended for production!**
* Install
```
npm install babel-register --save-dev
```
[FURTHER INFORMATION WILL BE UPDATED LATER]

## babel-node
**This module is not recommended for production!**


[FURTHER INFORMATION WILL BE UPDATED LATER]

## Babel configuration

Babel doesn't transpile any code if you did not explicitly tell it what to do. 
### .babelrc
```
{
    "presets": [],
    "plugins": []
}
```
Tell Babel to transpile from ES6 to ES5 by using this

```
npm install babel-preset-es2015 --save-dev
```


