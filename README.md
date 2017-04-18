# vue-fullpage

[效果展示界面](http://shenqiangqiang.github.io/vue-fullpage/)

使用vue.js制作的一个fullpage模板，可以通过修改配置，添加任意数量的page，支持滚轮和触摸滚动

## 运行方式：

``` bash
# 安装依赖
npm/cnpm/yarn install

# 本地开发服务器
npm run dev

# 打包导出
npm run build
```

## 效果演示


## 配置说明

在App.vue中修改data函数返回的内容，即为修改相应的配置。现在可以配置两个属性：currentPage和options

- currentPage:
表示当前显示的页面，通过设置currentPage可以改变初始显示的界面

- arrowsType:
表示页面控制器的上下箭头显示类型：no（不显示箭头）、normal（显示箭头）、animate（显示有动画效果的箭头）

- options:
该属性是一个数组，数组的每一项都是一个对象，通过设置对象内的值，可以改变对应的page组件的样式

1. background: 表示相应page的背景样式

2. color: 表示相应page的文字颜色（可以手动设置css样式覆盖）

3. isCenter: 表示相应page的内容是否居中（水平和垂直都包括）

4. beforeLeave() 该方法表示在离开当前页面前所做的操作（参数为当前页面的vue组件实例）

5. afterEnter() 方法表示在进入当前页面后所做的操作（参数为当前页面的vue组件实例）