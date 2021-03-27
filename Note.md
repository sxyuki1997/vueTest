# 前端知识点

<!-- > test -->

## 1. MVC与MVVM

```
MVC:
- Model: 存放数据模型
- View: 视图层
- Controller: 接受数据请求
当Controller接收到请求后,更新model的数据,model再针对dom进行操作,进行view的更新

MVVM:
- Model
- View
- View Model
View Model接受数据请求,更新model的数据,同时更新view视图,进行dom的渲染,实现了双向绑定的效果
```

## 2. v-model实现双向绑定原理
```
vue2.0是通过Object.defineProperty给对象属性设置get和set方法来实现数据实时更新与展现的
当用户输入发生改变时,首先利用get获取当前值,随后给相应元素的value赋值set更新,最后渲染dom
```

## 3. Vue的生命周期的理解
``` 
Vue的生命周期: 一个Vue的实例从创建到销毁的过程.
- beforeCreate 实例被创建前执行,数据未加载
- created 实例已被创建,初始化数据,dom未加载
- beforeMount 虚拟dom已创建,数据渲染之前,最后一次更改数据
- mounted dom已渲染
- beforeUpdate 重新渲染前触发
- updated 数据已更新,页面重新渲染
- beforeDestroy 实例销毁前,此时实例还存在
- destroyed 实例已销毁
```

## 4. for...in 与 for... of的区别
```
for...in遍历的是数组的索引（即键名），而for...of遍历的是数组元素值
```

## 5. $nextTick的作用
```
用于下次dom循环更新后执行延迟回调
在修改数据之后使用$nextTick可以在回调后获取更新后的dom
```

## 6. JS的基本类型，和引用类型，区别
```
- 基本类型: number，string，boolean，null，undefined
（1）基本类型的访问是按值访问的，就是说你可以操作保存在变量中的实际的值
（2）我们不能给基本类型添加属性和方法
（3）基本类型的变量是存放在栈区的（栈区指内存里的栈内存），栈区包括了 变量的标识符和变量的值。


- 引用类型: function，object，array
（1）引用类型的值是按引用访问的
（2）引用类型可以拥有属性和方法，并且是可以动态改变的。
（3）引用类型的存储需要内存的栈区和堆区（堆区是指内存里的堆内存）共同完成，栈区内存保存 变量标识符 和 指向堆内存中该对象的指针

```
## 7. Computed和methods区别
```
首先，对于最终的结果，两种方式是相同的，
针对computed，计算属性是基于它们的依赖进行缓存的，只有在其相关依赖改变时才会重新求值。
针对method，只要重新渲染，method调用总会执行该函数
```

## 8. Computed和watch
```
Computed是基于数据之上的对数据的一些计算操作
Watch是当特定的一个数据发生变化时，进行回调操作
```

## 9. Vue中的data为什么必须是函数？
```
对象属于引用类型，当修改其中一个属性时，会影响到所有vue实例的数据。
如果data是一个函数，返回一个对象，那么每一个实例的data对象都是互相独立的，不会相互影响。
```

## 10. html的语义化标签