# sham-ui-templates loader for webpack

```
npm install shamui-templates-loader --save
```

## Usage

```js
module.exports = {
  ...
  module: {
    loaders: [
      {
        test: /\.sht/,
        loader: 'sham-ui-templates-loader'
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