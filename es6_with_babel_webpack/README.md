# ES6 development with Babel and Webpack

## Reference
https://florianbrinkmann.com/en/4197/webpack-and-babel/

## Setup babel
* Create file *.babelrc* in the root folder of project:
```
{
  "presets": ["env"]
}
```

* Babel config

```
{
  "presets": [
    [
      "env",
      {
        "targets": {
          "browsers": ["last 2 versions", "safari >= 7"]
        }
      }
    ]
  ]
}
```

* Build with babel

```
babel . -d build
```
---

## Setup webpack
```
npm install webpack babel-loader --save-dev
```
 Create *webpack.config.js* file in root folder