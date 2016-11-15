```javascript
  //获取当前时间 实例化一个对象  
  var now = new Date();
  console.dir(now);
  console.log(now.getSeconds);
  
  //延迟五秒以后再吃输出一个date
  
  setTimeout(function(){
  console.log(newTime);
  console.log(newTime.getSeconds());
  },1000);
  
  /**
  *创建app now 的newtime的两个对象
  *它们包含的属性方式都是一致 值不同**/
  /**
  *methodName方法名  args1 args2 参数名
  *function methodName(argers,args2...){
  方法体 方法的内容
  return xxx
  }***/
  
  function Duck(name,color){
  this.name=name;
  this.color=color;
  this.walk = function(){
    console.log(this.color+'颜色的鸭子'+this.name+'.走起来');
    }
    this.eat =fuction(){
    console.log(this.color+'颜色的鸭子 walk'+this.name+',再吃东西');
    }
  }
  
  //创建jack 创建后的对象进行属性修改曹邹后不印象其他创建的对象
  var jack =new Duck('jack','黄');
  jack.walk();
  jack.legs =1;
  
  //创建calser
  
  var caler = new Duck('caler','白');
  caler.eat();
  caler.eyes =1;
 
 function walk(obj){
 console.log(obj.color+'颜色的鸭子'+ovj.name+'走起来');
 }
 function eat(ovj){
 console.log(obj.color+'颜色的鸭子'+obj.name+'吃东西');
 }
 var oldDuck={};
 oldDuck.name='jack';
 oldDuck.color='黄';
 walk(oldDuck);
 eat(oldDuck);
 
 
 
 //接下来总结下:
 /**
  *面向过程方式 需要定义变量 容易出现变量名称的重复问题
  *代码重用率比较低
  *结构不是很清晰
  *实现很简单代码容易看得懂
  *在实现一些简单的处理逻辑建议使用
  
  
  * 面向对象方式
  * 对象定义后可以重复使用
  * 对象定义之前需要把对象包含哪些属性和方法思考完全
  * 代码结构清晰 代码可读性强
  * 需要担心变量和方法重名的问题
  * 实现起来比较复杂,在实现的 时候尽量把对象相关的方法和属性定义的完整!!!!!!****************/
```
