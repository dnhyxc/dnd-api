## react-dnd

### react-dnd 简介

1，react-dnd 是 react 高阶组件，使用的时候只需要使用对应的 API 将目标组件进行包裹，即可实现拖动或接受拖动元素的功能。

### react-dnd 安装

```js
  yarn add react-dnd react-dnd-html5-backend immutability-helper

  npm install --save react-dnd react-dnd-html5-backend immutability-helper
```

### react-dnd API

1，`useDrag`：用于将当前组件用作拖拽源的钩子。

2，useDrag 参数：

> item：必填，一个普通的 JS 对象，描述了要拖动的数据。
>
> spec：必选，一个普通的 JS 对象，上面有一些允许的方放，它描述了拖动源如何对拖动事件做出反应。
>
> previewOptions：可选，描述拖动预览选项的普通 JS 对象。
>
> options：可选，一个普通的对象。
>
> begin(monitor)：可选，拖动操作开始时触发。
> 
> end(item, monitor)：可选，当拖动停止时，end 被调用。
> 
> canDrag(monitor)：可选，使用它来指定当前是否允许拖动。
>
> isDragging(monitor)：可选，默认情况下，只有启动拖动操作的拖动源才被视为拖动。
>
> collect：可选，具有收集功能，它应该返回道具的简单对象，并以返回注入到组件中，它接收两个参数，monitor 和 props。

2，useDrag 返回值：

> index 0：包含来自 collect 函数的收集属性的对象，如果 collect 未定义函数，则返回一个空对象。
>
>
>
>
>
>
>