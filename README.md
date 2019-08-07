# learning-Vue.js
深入学习Vue.js以及相关生态
![learning-Vue.js](http://assets.processon.com/chart_image/5d397b9ee4b0d11c8910c8eb.png)

## 学习资源

1. [Vue.js 官网](https://cn.vuejs.org/)
2. [Vue.js 源码解析](https://github.com/answershuto/learnVue)
3. [Vue 技术揭秘](https://ustbhuangyi.github.io/vue-analysis)
4. [vue-design](https://github.com/HcySunYang/vue-design)
5. 《深入浅出 Vue.js》

## Vue.js 基础

- 安装

1. Vue Devtools(Vue 开发功能，在浏览器中更好的审查和调试 Vue 应用)
2. 如何使用 Vue.js?(Vue.js 的安装方式)
3. 对于不同构建版本的解释？

- 介绍
  
1. Vue.js 是什么
2. 起步
3. 声明式渲染
4. 条件与循环
5. 处理用户输入
6. 组件化应用构建（PS:与自定义元素的关系？）

- Vue 实例

1. 创建一个 Vue 实例
2. 数据与方法
3. 实例生命周期钩子
4. 生命周期图示

> Vue 实例生命周期流程以及各个钩子函数的原理及用途

- 模板语法

1. 插值
2. 指令
3. 缩写

> 内置指令的使用及原理，动态参数与修饰符重点关注下使用场景

- 计算属性与侦听器
  - 什么是计算属性

    1. 基础例子
    2. 计算属性缓存 vs 方法
    3. 计算属性 vs 侦听属性
    4. 计算属性的 setter

  - 侦听器 

> computed 与 watch 使用场景

- Class 与 Style 绑定
  - 绑定 HTML Class
    - 对象语法
    - 数组语法
    - 用在组件上
  - 绑定内联样式
    - 对象语法
    - 数组语法
    - 自动添加前缀
    - 多重值

> 与 CSS 相关的功能是弱项，需要着重关注这一块的解决方案

- 条件渲染
  - v-if
  - v-show
  - v-if vs v-show

> 用 key 管理可复用的元素