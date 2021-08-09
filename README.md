<p align="center" style="text-align:center">
    <img src="./illustration.svg" alt="illustration" width="100"/>
</p>

# SCSS coding helpers

> Must have scss coding helper 

### Install

```shell
npm i scss-coding-helpers
```

### Initialization

#### SCSS File

Import to main scss file, or to need single .scss file

```scss
@import "~scss-coding-helpers";
```

#### Webpack 

* Install dependencies loaders

```shell
npm i -D css-loader sass-loader style-resources-loader 
```

* Include scss-coding-helpers index.scss file to your all .scss files with style-resources-loader
```js
module.exports = {
    module: {
            rules: [
                {
                    test: /\.scss$/,
                    use: [
                        {
                            loader: 'css-loader',
                            options: {
                                sourceMap: true,
                            },
                        },
                        {
                            loader: 'sass-loader',
                            options: {
                                sourceMap: true,
                            },
                        },
                        {
                            loader: 'style-resources-loader',
                            options: {
                                patterns: [
                                    path.resolve(__dirname, 'node_modules/scss-coding-helpers/index.scss')
                                ]
                            }
                        }
                    ]
                }
            ]
    }
}
```

### Documentation

Use <a href="https://scss-coding-helpers.vercel.app/" target="_blank">documentation</a> for quick start

## Author

webster6667
