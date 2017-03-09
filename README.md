# BootStrap学习中。。。
一、BootStrap的排版：<br>
## point-1<br><br>
.col-lg-1, .col-lg-10, .col-lg-11, .col-lg-12, .col-lg-2,
.col-lg-3, .col-lg-4, .col-lg-5, .col-lg-6, .col-lg-7,
.col-lg-8, .col-lg-9, .col-md-1, .col-md-10, .col-md-11,
.col-md-12, .col-md-2, .col-md-3, .col-md-4, .col-md-5,
.col-md-6, .col-md-7, .col-md-8, .col-md-9, .col-sm-1,
.col-sm-10, .col-sm-11, .col-sm-12, .col-sm-2, .col-sm-3,
.col-sm-4, .col-sm-5, .col-sm-6, .col-sm-7, .col-sm-8,
.col-sm-9, .col-xs-1, .col-xs-10, .col-xs-11, .col-xs-12,
.col-xs-2, .col-xs-3, .col-xs-4, .col-xs-5, .col-xs-6,
.col-xs-7, .col-xs-8, .col-xs-9 {<br>
    position: relative;<br>
    min-height: 1px;<br>
    padding-right: 15px;}<br><br>
注意每一列左右都有15px的padding。<br><br>
## point-2<br><br>
class="container":<br>会根据实际的屏幕尺寸，调整width的大小。<br>
.container {<br>
    padding-right: 15px;<br>
    padding-left: 15px;<br>
    margin-right: auto;<br>
    margin-left: auto;<br>
}<br>
.row {<br>
    margin-right: -15px;<br>
    margin-left: -15px;<br>
}<br>注意container也有15px的padding，但是row的-15px抵消了container和col同时的15pxpadding。<br><br>
## point-3<br><br>
如果每一列不为其设置四中屏幕大小的类:<br>例:只设置了class="col-md-6",则当屏幕小于md规定的尺寸时,
所有列会触发float:left属性。
## point-4:导航条部分：
container-fluid:类似于100%宽度。<br>
padding-right: 15px;<br>
    padding-left: 15px;<br>
    margin-right: auto;<br>
    margin-left: auto;<br><br>
一般用在导航条的最外层<nav>标签上的:

.navbar {

    position: relative;
    
    min-height: 50px;
    
    margin-bottom: 20px;
    
    border: 1px solid transparent;
    
}

.navbar-default {

    background-color: #f8f8f8;
    
    border-color: #e7e7e7;
    
}

.navbar-static-top :

类即可创建一个与页面等宽度的导航条，它会随着页面向下滚动而消失。


.navbar-fixed-top :

类可以让导航条固定在顶部;

此时需要给body加一个padding-top,以防挡住内容。


.navbar-fixed-bottom :

类可以让导航条固定在底部

此时需要给body加一个padding-bottom


.navbar-inverse {:会影响其中所有有关组件的颜色。

    background-color: #222;
    
    border-color: #080808;
    
}

