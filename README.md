# 简介
Facebook推出，2013年开源。react16.1之后被称为`React Fiber`，因为16.1版本之后的react底层算法做了修改。
# 组件
react组件里面必须要有函数render。  
父组件通过属性的方式向子组件传递数据
# JSX语法
可以在jsx语法里面写`js表达式`,不能写js语句
# 性能优化研究
## 概念
`首屏时间 DOMContentLoaded`   
* 工信部《宽带速率的测试方法用户上网体验》：浏览器显示第一屏页面所消耗的时间，以800x600像素尺寸为标准，从开始加载到浏览器页面显示高度达到600像素且此区域有内容显示的时间。  
* 用户能够看到区域内所有元素加载完的时间，这里指的是chrome浏览器Network面板下的`DOMContentLoaded`的秒数。  
* 2s以内优秀，5s以内用户可以接受，10s以上不可容忍  
* DOMContentLoaded 的触发不需要等待图片等其他资源加载完成  

`Loaded`  
* 页面上所有的资源（图片，音频，视频等）被加载以后才会触发load事件
* 页面的load事件会在DOMContentLoaded被触发之后才触发
## 预加载
# Vue框架性能优化
## 路由懒加载
