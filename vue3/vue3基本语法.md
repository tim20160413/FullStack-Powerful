# Vue3基本语法

* 路径书写
  ```
  ./：表示相对路径，具体代表当前目录下的同级目录，遵从的是从后往前找文件
  @/：表示的是相对路径，@ 代表就是 src 目录，遵从的是从前往后找
  例如:import store from '@/example/store/index'
      import install from './packages/install'
  ```

* import ... from ..
  <br>https://blog.csdn.net/fyyyr/article/details/83657828
