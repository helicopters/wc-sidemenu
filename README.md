## wc-drawer

基于 Vue 的抽屉效果. 

## 描述

唤起: 通过页面上的一个 三明治 唤起
可以从左边或者右边唤起. 

唤起效果: 
content 动, drawer 不动
content 不动, drawer 动
content 动, drawer 动. 

drawer: 可以滚动, 点击不会导致关闭 drawer
此时 content 不能滚动
drawer 和 content 都不能左右滑动. 

关闭: 点击 x 按钮, 或者主页面的任意地方. 


## step
之前的思路, 我是想着通过一个变量来控制, 还是暂时不要这么做, 提供两个函数, 让用户自己控制显示隐藏. 
然后 content 动这个行为, 也由用户自己控制. 用户自己控制 content 动与否. 

我们的 drawer 只负责控制自己的动与否。 

如果 content 自己动的话, 需要我们提供 drawer 的宽度, 同时 content 需要自己实现一个函数. 
不能这么做. 
所以还是要让 drawer 来控制. 
drawer 控制, 我们要提供所有需要移动的标记. 

然后同时需要一个 mode, 来控制 content 和 drawer 的联动方式. 

































