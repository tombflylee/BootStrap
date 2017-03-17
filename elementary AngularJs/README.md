## BootStrap+AngularJs——购物车:
1、angular.forEach(obj, iterator, [context]);

描述:

循环对obj对象的每个元素调用iterator,obj对象可以是一个Object或一个Array.

Iterator函数调用方法: iterator(value, key, obj),其中obj是被迭代对象，key是obj的property key或者是数组的index，value就是相应的值啦. (此函数不能够迭代继承的属性.)

例子:

 $scope.totalPrice=function(){
    var totalPrice=0;
    angular.forEach($scope.cart,function (value) {
        totalPrice+=value.quantity * value.price;
    })
    return totalPrice;
}
