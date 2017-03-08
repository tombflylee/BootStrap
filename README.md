# BootStrap学习中。。。
一、BootStrap的排版：<br>
<em>point-1</em><br><br>
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
<em>point-2</em><br><br>
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
<em>point-3</em><br><br>
如果每一列不为其设置四中屏幕大小的类:<br>例:只设置了class="col-md-6",则当屏幕小于md规定的尺寸时,
所有列会触发float:left属性。
