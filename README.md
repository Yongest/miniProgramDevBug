# 小程序开发遇到的坑 #

### 1.遮罩层遮盖不住textare ，点击遮罩层可以在文本域输入 ##

### 2.指令不能用，过滤器需要使用 `.wxs` 文件,且`.wxs`文件中只能使用es2015语法，获取时间对象只能用getDate()，写入 `<wxs module="common" src='../../utils/common.wxs'></wxs>  common.fixed(something)` ##

### 3.部分css样式不能用 ##

### 4.右上角分享功能需要每个页面都调用 ##

### 5.获取地理位置需要在`app.json` 里面 `permission` ##

### 6.navigator  需要有url ##

### 7.利用`swiper、scroll-view 组件`可以制作左右滑动并且上拉加载的 `tab功能`, `scroll-view有自己的触发滑到底部的事件，需要定义一个高度` ##

### 8.常用功能封装，ajax,支付，toast，电话等，对常用css抽离，例如颜色，字体，margin,border,背景色，圆角padding，箭头等,使用的时候只需要在标签中加类名，不需要再次写样式，提高开发效率。 ##

### 9.封装常用的组件，上拉加载状态显示。 ##

### 10.tab栏图片需要用微信的图片，不支持网络图片 ##

### 11.tab栏图片需要用微信的图片，不支持网络图片 ##

### 12. button 原样式较多，可以使用view替代 ##

### 13. 表单数据双向绑定问题。需要配合

### 14. storage存储问题，退出小程序不会自动清除storage，需要想办法。

### 15. 用户登录功能。
### 16. 获取data里面的数据，需要这样 `this.data.msg`,因为 `msg`没有赋值到根实例上面，而是放在data中。
### 17.app.wxss 不作用于独立包，组件。如组件中需要公共样式，需要使用 `@import '/app.wxss';` 导入
### 18，wx:for  循环,默认值为item，索引为index,可以改变，建议设置key，一般为两种方式wx:key="unique"或wx:key="*this"
### 19.函数调用传值不方便。只能写函数名，不能传值。

### 20.过滤器中，`string.substr(5,11)` 不起作用 替换方法，`string.substring()`
