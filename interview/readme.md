
1. Zepto如何理解的？和jquery什么区别？

* Zepto移动端的jquery。
* Zepto只能用在移动端
* Jquery既可以用在PC端又可以用在移动端。由于jquery库太大了所以移动端用的少。
* Zepto相比jquery多了一些手势相关事件
* Zepto解决了移动端点击事件300ms延迟的问题。  （fastclick.js也是解决300ms延迟问题）
* Zepto基于模块  很小轻量级  用到那个引入那个

2. zepto与jquery冲突的解决？
 
 * jquery有一个方法叫noConflict() ,可以把jquery的$改掉。

       var jq=$.noConflict();

        这个时候用jq来代替jquery的$吧。

* zepto的符号改掉

    window.$$=window.Zepto = Zepto

   在zepto里加入这一行代码，就可以用$$来代替zepto里的$了。当然也可以选择其他符号来代替。