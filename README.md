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

- 列表渲染
  - 用 v-for 把一个数组对应为一组元素
  - 在 v-for 里使用对象
  - 维护状态
  - 数组更新检测
    - 变异方法 (mutation method)
    - 替换数组
    - 注意事项
  - 对象变更检测注意事项
  - 显示过滤/排序后的结果
  - 在 v-for 里使用值范围
  - 在 `<template>` 上使用 v-for
  - v-for 与 v-if 一同使用
  - 在组件上使用 v-for

> v-for 与 v-if 一起使用时的注意事项，数组的变更检测

- 事件处理
  - 监听事件
  - 事件处理方法
  - 内联处理器中的方法
  - 事件修饰符
  - 按键修饰符
    - 按键码
  - 系统修饰键
    - .exact 修饰符
    - 鼠标按钮修饰符
  - 为什么在 HTML 中监听事件？

> 对于事件这一块，应该结合原生事件理解，在实际开发中用到的频次最多的就是 click 事件了，有比较的知识盲点

- 表单输入绑定
  - 基础用法
    - 文本
    - 多行文本
    - 复选框
    - 单选按钮
    - 选择框
  - 值绑定
  - 修饰符
    - .lazy
    - .number
    - .trim
  - 在组件上使用 v-model

> 在组件上使用 v-model 的方式日常开发很少用，对于此方式的使用场景以及原理需要重点关注

- 组件基础
  - 基本示例
  - 组件的复用
    - data 必须是一个函数
  - 组件的组织
  - 通过 Prop 向子组件传递数据
  - 单个根元素
  - 监听子组件事件
    - 使用事件抛出一个值
    - 在组件上使用 v-model (重点)
  - 通过插槽分发内容
  - 动态组件
  - 解析 DOM 模板时的注意事项
  
> 插槽分发需要深入学习其使用场景及原理