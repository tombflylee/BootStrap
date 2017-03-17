## BootStrap+AngularJs——购物车:
1、angular.forEach(obj, iterator, [context]);

描述:<br>
循环对obj对象的每个元素调用iterator,obj对象可以是一个Object或一个Array.

Iterator函数调用方法: iterator(value, key, obj),其中obj是被迭代对象，key是obj的property key或者是数组的index，value就是相应的值啦. (此函数不能够迭代继承的属性.)

例子:

 $scope.totalPrice=function(){<br>
    var totalPrice=0;<br>
    angular.forEach($scope.cart,function (value) {<br>
        totalPrice+=value.quantity * value.price;<br>
    })<br>
    return totalPrice;<br>
}

2、data-ng-click="x.quantity=x.quantity-1"

注意：
1、不能写{{}},{{}}写在html内容中的。<br>
2、不能写x.quantity--

3、在input标签内输入的内容,会被认为是string类型,所以在计算总数量时候,将输入的值转换为number类型。

   Number(value.quantity,10);
   
   代码展示：https://codepen.io/tombflylee/pen/BWmYyX?editors=1010
