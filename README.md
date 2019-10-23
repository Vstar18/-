# 前端知识网
tomarrow is anthoer day
细节见成败

### JS
### CSS
### 三大框架
### 前端工程化
### webpack
  - 五大基础概念
    1. entry 入口
      - 多入口：对象写法
        ```
        entry: {
          app: './src/app.js',
          vendors: './src/vendors.js'
        }
        ```
        优点：可扩展性强，即可重用，可和其他配置组合使用（webpack-merge合并）
       - 单一入口 ：
       ```
       const config = {
         entry: './path/to/my/entry/file.js'
       };
       ```
    2. output 出口
      >  属性告诉 webpack 在哪里输出它所创建的 bundles，以及如何命名这些文件
    3. loader 
      - 作用：用于模块的源代码进行转换成js（css，img等都可以处理成js，因为webpack只认识js文件）
      - 使用方式： 
        1. 内置配置，我们常用的webpack.config文件
        2. CLI，shell命令
        ```
        webpack --module-bind jade-loader --module-bind 'css=style-loader!css-loader'
        ```
        3. import语句显示的指明
          通过所有规则及使用 !
         ```
         import Styles from 'style-loader!css-loader?modules!./styles.css';
         ```
         > 推荐使用内置配置的方式
         1. 可以减少源码量
         2. 可以在发生问题的使用迅速定位
    4. plugin 插件
    5. mode 模式
### NodeJS
### PWA
### Service Work
### Http
### [算法](https://github.com/Vstar18/FE-knowledge-algorithm)
