# Vue

> Vue 教程 [https://www.vuefe.cn/v2/guide/index.html](https://www.vuefe.cn/v2/guide/index.html)
> 
> Vue API [https://www.vuefe.cn/v2/api/](https://www.vuefe.cn/v2/api/)
> 
> Vuex [https://vuex.vuejs.org/zh-cn/intro.html](https://vuex.vuejs.org/zh-cn/intro.html)
> 
> Vue Router [https://router.vuejs.org/zh-cn/essentials/getting-started.html](https://router.vuejs.org/zh-cn/essentials/getting-started.html)
> 
> Vue SSR [https://ssr.vuejs.org/zh/](https://ssr.vuejs.org/zh/)

注意事项

- 同一类型事件只能绑定一次，如 change。
- data 中的属性提前创建，否则不被监听，dom 也是如此。
- 不要在选项属性或回调上使用箭头函数。
- {{ name }} 插值时不能加入 html 标签。
- 不能绑定空内容。
- updated 生命事件，初次加载不执行，更新时才执行。
- computed 如果定义的属性初始化时没有被使用，则永远不会执行该函数。
- v-if 用注释替代其位置，v-show 用 display:none 隐藏显示。
- 子组件内部，需要顶级挂载节点，且只能有一个。
- input 等表单控件修改后，需要手动同步 vue 数据。
- 使用插件时，需要通过 jQuery 绑定 change 事件来获取事件。插件使用 js 修改值时，不会触发浏览器的 change 事件，只会触发 jQuery 模拟的事件。
- Vuex 一个 input 如果原值是 a，修改后，再赋值为 a。由于虚拟 DOM 的值没有改变，顾不触发更新，导致 input 的值为修改后的值，并非最后赋值的a。

基础

- [双向绑定原理](Base/theory.md)
- [生命周期](Base/lifecycle.md)
- [模板语法](Base/template.md)
- [计算属性和观察者](Base/计算属性和观察者.md)
- [Class 与 Style 绑定](Base/Class与Style绑定.md)
- [条件渲染](Base/条件渲染.md)
- [列表渲染](Base/列表渲染.md)
- [事件处理](Base/事件处理.md)
- [表单输入绑定](Base/表单输入绑定.md)

组件

- [定义组件模板的7种方法](Base/Component/定义组件模板的7种方法.md)
- [使用方法](Base/Component/使用方法.md)
- [Prop](Base/Component/Prop.md)
- [自定义事件](Base/Component/自定义事件.md)
- [插槽分发内容](Base/Component/插槽分发内容.md)
- [杂项](Base/Component/杂项.md)

过渡 & 动画

- 进入/离开 & 列表过渡
- 状态过渡

可复用性 & 组合

- [混合](Reuse/混合.md)
- [自定义指令](Reuse/自定义指令.md)
- [渲染函数 & JSX](Reuse/渲染函数&JSX.md)
- [插件](Reuse/插件.md)
- [过滤器](Reuse/过滤器.md)
- [深入响应式原理](Reuse/深入响应式原理.md)

规模化

- [Vuex](Vuex.md)
- [Vue Router](Vue-Router.md)
- Vue SSR
