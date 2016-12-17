# template-file-loader
helps you load template file, supported by consolidate

## Usage
``` js
{
  test: /\.pug$/,
  loader: 'vue-template-es2015-loader!template-file-loader&raw' // compile `.pug` file to html then pass plain text to `vue-template-es2015-loader`
}
```

You can specific an engine (should be supported by [consolidate](https://www.npmjs.com/package/consolidate)) as
following: `template-file-loader?engine=ejs`, or `template-file-loader` will get engine from the extname of file.

With removing option `row`, you will get a valid js module: `module.exports = "Your Template File Content"`

---

That's all.
