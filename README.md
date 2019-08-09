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

## 深入了解组件

- 组件注册
  - 组件名
    - 组件名大小写
  - 全局组件
  - 局部组件
  - 模块系统
    - 在模块系统中局部注册
    - 基础组件的自动化全局注册

> 组件命名的规范统一，自动化全局注册基础组件

- Prop
  - Prop 的大小写
  - Prop 类型
  - 传递静态或动态 Prop
    - 传递一个数字
    - 传递一个布尔值
    - 传递一个数组
    - 传递一个对象
    - 传递一个对象的所有属性
  - 单向数据流
  - Prop 验证
    - 类型检查
  - 非 Prop 的特性
    - 替换/合并已有的特性
    - 禁用特性继承
  - 自定义事件
    - 事件名
    - 自定义组件的 v-model
    - 将原生事件绑定到组件
    - .sync 修饰符

> 如何传递一个对象的所有的属性

- 插槽
  - 插槽内容
  - 编译作用域
  - 后备内容
  - 具名插槽
  - 作用域插槽
   - 独占默认插槽的缩写语法
  - 解构插槽 Prop
  - 动态插槽名
  - 具有插槽的缩写
  - 其他示例
  - 废弃了的语法
    - 带有slot特性的具名插槽
    - 带有slot-scope特性的作用域插槽

> 插槽的基础用法以及高级用法，废弃语法的替换

- 动态组件 & 异步组件
  - 在动态组件上使用 keep-alive
  - 异步组件
    - 处理加载状态

> 动态组件的使用场景以及更好的使用异步组件

- 处理边界情况
  - 访问元素 & 组件
    - 访问根实例
    - 访问父级组件实例
    - 访问子组件实例或子元素
    - 依赖注入
  - 程序化的事件监听器
  - 循环饮用
    - 递归组件
    - 组件之间的循环饮用
  - 模板定义的替代品
    - 内联模板
    - X-Template
  - 控制更新
    - 强制更新
    - 通过 v-once 创建低开销的静态组件

> 这里需要进一步深入的理解，有些地方一知半解

## 过渡 & 动画

- 进入/离开 & 列表过渡
  - 概述
  - 单元素/组件的过渡
    - CSS 过渡
    - CSS 动画
    - 自定义过渡的类名
    - 同时使用过渡和动画
    - 显性的过渡持续时间
    - JavaScript 钩子
  - 初始渲染的过渡
  - 多个元素的过渡
    - 过渡模式
  - 多个组件的过渡
  - 列表过渡
    - 列表的进入/离开过渡
    - 列表的排序过渡
    - 列表的交错过渡
  - 可复用的过渡
  - 动态过渡
- 状态过渡
  - 状态动画与侦听器
  - 动态状态过渡
  - 把过渡放到组件里
  - 赋予设计以生命

> 这一块很少用到，属于知识盲区

## 可复用性 & 组合

- 混入
  - 基础
  - 选项合并
  - 全局混入
  - 自定义选项合并策略
- 自定义指令
  - 简介
  - 钩子函数
  - 钩子函数参数
    - 动态指令参数
  - 函数简写
  - 对象字面量

> 自定义指令在开发中遇到实际的业务场景，需要探索更多的应用场景，遇到的问题可以通过查文档很好的解决

- 渲染函数 & JSX
  - 基础
  - 节点、树以及虚拟DOM
    - 虚拟DOM
  - createElement 参数
    - 深入数据对象
    - 完整示例
    - 约束
  - 使用 JavaScript 代替模板功能
    - v-if 和 v-for
    - v-model
    - 事件 & 按键修饰符
    - 插槽
  - JSX
  - 函数式组件
    - 向子元素或者自组件传递特性和事件
    - slots() 和 children 对比
  - 模板编译

> 这一块用到的比较少，一般业务都是通过 template 形式写的，需要理解渲染函数的原理以及 JSX 的使用场景

- 插件
  - 使用插件
  - 开发插件

> 插件的使用与开发比较常用，这一块稍微熟悉一点，需要进一步搞清楚插件开发的各个细节

- 过滤器

## 工具

- 单文件组件
  - 介绍
    - 怎么看待关注点分离
  - 起步
    - 例子沙箱
    - 针对刚接触 JavaScript 模块开发系统的用户
    - 针对高级用户
- 单元测试
  - 简单的断言
  - 编写可被测试的组件
  - 断言异步更新
- TypeScript 支持
  - 发布为 NPM 包的官方声明文件
  - 推荐配置
  - 开发工具链
    - 工程创建
    - 编辑器支持
  - 基本用法
  - 基于类的 Vue 组件
  - 增强类型以配合插件使用
  - 标注返回值
- 生产环境部署
  - 开启生产环境模式
    - 不使用构建工具
    - 使用构建工具
  - 模板预编译
  - 提取组件的 CSS
  - 跟踪运行时错误

> 对于单元测试与 TS 支持是进阶重点关注的点，需要进一步学习

## 规模化

- 路由
  - 官方路由
  - 从零开始简单的路由
  - 整合第三方路由
- 状态管理
  - 类 Flux 状态管理的官方实现
    - React 的开发者请参考以下信息
  - 简单状态管理起步使用
- 服务端渲染
  - SSR 完全渲染指南
  - Nuxt.js
  - Quasar Framework SSR + PWA

> 路由和状态管理在开发中时比较常用的，对于 SSR 和 PWA 在所属业务中并没有实际的使用场景，但也要有一定的了解，可以快速提供可用的解决方案

## 内在

- 深入响应式原理
  - 如何追踪变化
  - 检测变化的注意事项
  - 声明响应式属性
  - 异步更新队列

## 更多

- 对比其他框架
- 加入 Vue.js 社区
- 认识团队

> 对比其他框架内容需要详细了解一下，对于技术选型有一定的决策帮助，认识社区跟团队，可以更好的了解生态的发展趋势