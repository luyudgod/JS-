# JS-学习路线记录
1.输出一个字符串. 
     使用win下的方法alert()，生成一个网页弹窗。用来输出消息

2.在console里输出日志. 
     使用js提供的console对象下的log()方法来打印控制台信息

3.定义一个变量，类型为Sting， 使用var标识符创建一个变量，并进行初始化操作. 
      var a="1" /此初始化操作 为定义一个标识符为a的变量 并进行复制操作，把1复制给a 
      JS是弱类型语言，申明一个变量时无需提前定义变量类型 定义变量时还需根据作用域来判断使用的标识符，和变量的定义位置，
      有时还需注意声明提升  函数和变量的提升

4.熟悉语言的各数据类型
      bool
      string
      number
      char
      object
      arr[]
      function

5.数据类型转换
     string下的方法 string()函数是全局转换函数
     number()
     tostring属性 tonumber属性
     typeof() 可以用来查看当前数据的类型
     也可直接查看数据的构造函数，来区分数组，对象
    
6.判断 switch if 三元运算 if....else if
     switch的用法 break 
     if 的条件语句
     三元运算 a<b?1:2  ？号前做条件判断 符合则执行1 也就是true  反之则为2 也就是flase

7.循环 for for x in x  while do....while
     for(a,b,c){} a为循环执行前执行 b为循环中执行 也是for的条件判断 为ture时执行 为flase时停止 c为执行完一个周期时执行 后跟执行代码块
     for a in b 一般为遍历对象或者数组时应用的  我的理解是 a可以是执行次数记录 也可是内容的记录 而b为被执行的对象或数组
     while true  while循环 根据后面的条件表达式的值来决定是否执行循环操作 do while 和while差不多 不过要在判断前执行一次代码，然后再进行条件判断来决定是否再次执行
     特殊语句：continue  用来跳过一次循环迭代 break 用来跳过当前循环（如果未有标签的情况下）
 
8.创建函数
     函数（function） 比较重要的一环 函数的形参 返回值 调用 作用域  
     function a(b){return c}  如只有一行代码 则不需代码块 此处a为此函数的名称 b为此函数的形参 后跟代码块 调用函数 a()  在函数中使用var来定义变量属于局部变量 作用域仅限函数内
     return为函数返回值
     var a=function(){} 这是一个匿名函数 把函数名赋值给变量a
     函数还可以做对象的构造体

9.对象
     对象（object） JS中的所有数据都是一个对象 应该！ 
     对象的创建：var a={name:"value",name1:"value1"
                        name3:function(){}
                        }
     这之中有name属性和name3方法 调用 a.name=value a.name1=value1 a.name3()
     对象还可以用对象构造体来创体 对象构造体使用函数类型
     var newobject=function(a,b,c,d){
                   this.a=a
                   this.b=b
                   this.c=c
                   this.d=function(){}
                           //此为注释  this在这里指向本函数的形参 外部的话指向window的属性
                           }
10.JS中的严格模式
   严格模式中未声明的变量 直接赋值会被系统报错 返回:a is not defined

11.验证API
   验证输入的内容是否合法
   验证输入内容的类型 长度 大小
   验证方法有很多种

12.表单验证
   document.froms.value["frome表单name"]["表单下的属性name"] 可以用来取值来做判断 表单里的这个值是否为可用
   a = document.froms.value["a"]["b"]
   function a(){if(a!==null || a!==undefined || a!=="" || isNaN(a)){
          alert("符合所有条件")
          return true
   }else return flase;}
   onsubitm return a()
13.作用域
   let 可用来更改变量的作用域
   所有函数内部共用一个内部作用域

14.





//以上有很多需要补充的 大多数时间都在实践 所以很多东西都是根据我的记忆来写的，很零碎！！！
