## Template Reactjs with typescript

React v17.0.2 with TypeScript

_In this project we have basic settings to work with Typescript, Babel, images, CSS, SASS and Fast Refresh to avoid unnecessary state changes._

## **Used libs**

### **For cross platform environment variable**
* [cross-env](https://www.npmjs.com/package/cross-env)
### **Loaders for webpack rules**
* [babel-loader](https://www.npmjs.com/package/babel-loader)
* [css-loader](https://www.npmjs.com/package/css-loader)
* [file-loader](https://www.npmjs.com/package/file-loader)
* [sass-loader](https://www.npmjs.com/package/sass-loader)
* [url-loader](https://www.npmjs.com/package/url-loader)
### **SASS**
* [node-sass](https://www.npmjs.com/package/node-sass)
### **Image Optimizers**
* [imagemin-gifsicle](https://www.npmjs.com/package/imagemin-gifsicle)
* [imagemin-jpegtran](https://www.npmjs.com/package/imagemin-jpegtran)
* [imagemin-mozjpeg](https://www.npmjs.com/package/imagemin-mozjpeg)
* [imagemin-optipng](https://www.npmjs.com/package/imagemin-optipng)
* [imagemin-pngquant](https://www.npmjs.com/package/imagemin-pngquant)
* [imagemin-svgo](https://www.npmjs.com/package/imagemin-svgo)
* [image-minimizer-webpack-plugin](https://www.npmjs.com/package/image-minimizer-webpack-plugin)

### **Inject bundle**
* [html-webpack-plugin](https://www.npmjs.com/package/imagemin-svgo)

### **Fast refresh components**
* [@pmmmwh/react-refresh-webpack-plugin](https://www.npmjs.com/package/@pmmmwh/react-refresh-webpack-plugin)

### **Babel preset**
[@babel/preset-env](https://www.npmjs.com/package/@babel/preset-env)
[@babel/preset-typescript](https://www.npmjs.com/package/@babel/preset-typescript)
[@babel/preset-react](https://www.npmjs.com/package/@babel/preset-react)

### Babel config 

```js
//babel.config.js
module.exports = {
  presets: [
    "@babel/preset-env", //that allows you to use the latest JavaScript without needing to micromanage which syntax transforms
    "@babel/preset-typescript", // that allows you to use Typescript
    [
      "@babel/preset-react",
      {
        runtime: "automatic", // react refresh automatic. Default is classic
      },
    ],
  ],
};
```