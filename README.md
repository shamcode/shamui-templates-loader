# sham-ui-templates loader for webpack

```
npm install sham-ui-templates-loader --save
```

## Usage

```js
module.exports = {
  ...
  module: {
    rules: [
      {
        test: /\.sht$/,
        loader: 'sham-ui-templates-loader'
      },
      {
        test: /\.sfw$/,
        use: [
           { loader: 'babel-loader' },
           { 
             loader: 'sham-ui-templates-loader', 
             options: {
               asModule: false,
               asSingleFileWidget: true
             } 
           }
        ]
      }
    ]
  },
  ...
};
```

## Configuration 

Add `sham-ui` section to your `webpack.config.js`:

```js
'sham-ui': {
  globals: ['window'],
  transforms: [...]
}
```
