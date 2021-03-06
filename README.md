# mocha loader for webpack

## Usage

### Command Line

*Hint*: when using `!` in the bash command line, you must escape it by prepending a `\`

``` text
webpack-dev-server 'mocha!./my-client-tests.js' --options webpackOptions.js
```

``` text
enhanced-require 'mocha!./my-server-tests.js'
```

### webpack.config.js

When using `webpack.config.js`, simply prepend `mocha!` in front of the entry:

``` text
// webpack.config.js 
module.exports = {
    entry: 'mocha!./entry-file.js',
    output: {
        path: __dirname,
        filename: 'bundle.js'
    }
};
```

## License

MIT (http://www.opensource.org/licenses/mit-license.php)
