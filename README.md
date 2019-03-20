# vue_learning_record
vue 学习记录
## vue项目的前端优化和ios兼容性问题
### 低版本ios白屏问题：
     原因是：es6不兼容
     解决方法： npm install --save-dev babel-polyfill 
               webpack.base.conf里：
                   {
                       test: /\.js$/,
                       exclude: /node_modules/,
                       loader: "babel-loader"
                   }
