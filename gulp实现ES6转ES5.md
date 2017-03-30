# 通过gulp插件实现es6转es5

`npm install --save-dev gulp-babel`
### 安装 Gulp 上 Babel 的插件。

`npm install --save-dev babel-preset-es2015`
### 安装 Babel 上将 ES6 转换成 ES5 的插件。

 

 

### gulp 配置：

```
var gulp = require("gulp");
var babel = require("gulp-babel");

gulp.task("default", function () {
  return gulp.src("src/**/*.js")// ES6 源码存放的路径
    .pipe(babel()) 
    .pipe(gulp.dest("dist")); //转换成 ES5 存放的路径
});
```

babel配置：
在项目根路径创建文件 .babelrc。内容为
```
{
  "presets": ["es2015"]
}
``


