# Vue3基础

## 一、Vue3项目环境搭建
* 1、mac上安装npm, 通过node.js安装
  ```
    http://nodejs.cn/download/ 下载pkg包,安装
    查看安装成功:npm -v
    结果(参考):
    8.5.5
  ```

*(如果不是root权限,每条命令最前面加上sudo,例如sudo npm install webpack -g)*
* 2、安装webpack打包工具
  ```
  npm install webpack  -g
  ```
  
* 3、安装vue-cli脚手架，用于初始化vue项目
  ```
  npm install vue-cli -g
  查看安装成功:vue -v
  结果(参考):
  2.9.6
  ```

* 4、设置淘宝镜像(可选项,推荐)
  ```
  由于npm使用的是国外的中央仓库，所以有人说会比较慢，但是个人觉得还可以。
  跟maven一样，npm在国内也有自己的镜像仓库，如果觉得慢可以设置为国内的镜像仓库。
  npm install -g cnpm --registry=https://registry.npmmirror.com
  设置成功之后，npm命令将不能使用，取而代之的是cnpm。
  ```

## 二、Vue3项目快速构建
* 1、在用 Vue.js 构建大型应用时推荐使用 cnpm 安装，cnpm 能很好地和 Webpack 或 Browserify 模块打包器配合使用：
  ```
  最新稳定版
  $ cnpm install vue@next
  ```

* 2、Vue.js 提供一个官方命令行工具，可用于快速搭建大型单页应用。
  ```
  对于 Vue 3，你应该使用 npm 上可用的 Vue CLI v4.5 作为 @vue/cli。要升级，你应该需要全局重新安装最新版本的 @vue/cli：
  cnpm install -g @vue/cli
  安装完后查看版本:
  $ vue --version
  结果(参考):@vue/cli 4.5.11
  
  $ vue upgrade --next
  ```

* 3、使用vue init命令创建一个项目
  ```
  如果出现提示:
    Command vue init requires a global addon to be installed.
    Please run npm i -g @vue/cli-init and try again.
    
  可以使用:npm i -g @vue/cli-init 进行安装
  ```
  ```
  $ vue init webpack runoob-vue3-test
  这里需要进行一些配置，默认回车即可
  ? Project name runoob-vue3-test
  ? Project description A Vue.js project
  ? Author runoob <test@runoob.com>
  ? Vue build standalone
  ? Install vue-router? Yes
  ? Use ESLint to lint your code? Yes
  ? Pick an ESLint preset Standard
  ? Set up unit tests Yes
  ? Pick a test runner jest
  ? Setup e2e tests with Nightwatch? Yes
  ? Should we run `npm install` for you after the project has been created? (recommended) npm

     vue-cli · Generated "runoob-vue3-test".


  启动:
  $ cd runoob-vue3-test
  $ cnpm run dev
  成功执行以上命令后在浏览器访问 http://localhost:8080/，输出结果如下所示：
  ```

* 4、使用Vite构建vue项目(推荐)
  ```
  Vite 是一个 web 开发构建工具，由于其原生 ES 模块导入方式，可以实现闪电般的冷服务器启动。
  通过在终端中运行以下命令，可以使用 Vite 快速构建 Vue 项目，语法格式如下：cnpm init @vitejs/app <project-name>
  
  创建项目 runoob-vue3-test2：
  $ cnpm init @vitejs/app runoob-vue3-test2
  运行项目:
  $ cd runoob-vue3-test2
  $ cnpm install
  $ cnpm run dev
  成功执行以上命令在浏览器访问 http://localhost:3000/
  ```

## 三.安装其他
 * 1.安装vue-router
   ```
   npm install vue-router@4
   ```
  * 2.安装typescript
    ```
    npm install -g typescript
    ```

  
