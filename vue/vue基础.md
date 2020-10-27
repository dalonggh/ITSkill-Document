## 1.双向绑定，

## 2.组件化开发，（代码复用）,

## 3.模板语法：{{}}，
## 4.vue指令，修饰符，过滤器（工具函数）

## 5.条件语句：v-if和v-show，
(1)v-if的原理是根据判断条件来动态的进行增删DOM元素，
(2)v-show是根据判断条件来动态的进行显示和隐藏元素。
(3)v-for比v-if优先级高，

## 6.watch 和 computed 和 methods 区别是什么？
(1)当页面中有某些数据依赖其他数据进行变动的时候，可以使用computed（计算属性）。computed是具有缓存的，
(2)数据变化的同时进行异步操作或者是比较大的开销。watch为一个对象，
	键是需要观察的表达式，值是对应回调函数。值也可以是方法名，或者包含选项的对象。
(3)data中没有声明的数据可以在computed中使用，但是不能在watch中使用。
(4)在computed和watch方面，一个是计算，一个是观察。
		①计算是通过变量计算来得出数据。而观察是观察一个特定的值，
	根据被观察者的变动进行相应的变化。
(5)Methods是组件的方法。

## 7.Vue路由：

(1)标签导航：标签导航<router-link><router-link>是通过转义为<a></a>标签进行跳转，其中router-link标签中的to属性会被转义为a标签中的href属性；
(2)编程式导航：我们可以通过this.$router.push()这个方法来实现编程式导航，当然也可以实现参数传递，这种编程式导航一般是用于按钮点击之后跳转；

## 8.Vue路由守卫
(1)应用场景：在项目开发中每一次路由的切换或者页面的刷新都需要判断用户是否已经登录，
(2)应用例子：![在这里插入图片描述](https://img-blog.csdnimg.cn/20201022154410498.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dzRGFMb25n,size_16,color_FFFFFF,t_70#pic_center)
## 9.Vue生命周期钩子函数

钩子函数有8个，ajax获取数据在mounted（模板渲染完毕后）中执行。

* beforeCreate；
* created；
* beforeMount；
* mounted；
* beforeUpdate；
* updated；
* beforeDestroy；
* destroyed；
## 10.Vue组件之间通信（传值）

(1)使用$children获取子组件和父组件对象,(父传子)，

(2)通过props进行通信,(父传子)，
(3)使用$emit传递事件给父组件，父组件监听该事件，（子传父）,

(4)使用$parent.获取父组件对象，然后再获取数据对象，（子传父）
(5)Slot：插槽传值，
(6)使用事件总线，（任意组件）
(7)Vuex（仓库），（任意组件）

## 11.Vuex

(1)State，状态（数据）管理，
(2)Mutations，状态修改的方法（同步），
(3)Getters：状态的进一步加工，（相当于组件的computed），
(4)Actions，状态的异步操作，（ajax请求），

## 12.Vue实例属性或方法

(1)$refs：获取模板的中dom节点（元素），

(2)$route：获取路由传递的参数，

(3)$emit：向父级组件触发一个事件，

(4)$event：事件发生对象，

(5)$set：在vue中，给对象添加属性,

(6)$options：获取当前组件的属性（获取当前组件的name）
