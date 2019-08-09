# dom
    dom事件类
       基本概念：dom事件的级别
         dom0 element.onclick=function(){}
         dom2 element.addEventListener('click',function(){},false)
         dom3 element.addEventListener('keyup',function(){},false)
       dom事件模型
         捕获/冒泡 
       dom事件流
          捕获->目标阶段->冒泡
       描述dom事件捕获的具体流程
          window->document->html->body->...->目标
          冒泡相反
       event对象的常见应用
          event.preventDefalt()//阻止默认事件
          event.stopPropagation()//阻止冒泡
          event.stopImmediatePropagation()//阻止同一个元素其他事件的发生
          event.currentTarget//当前绑定的事件的元素
          event.target//当前点击元素
       自定义事件
        vareve= new Event('custome');
        ev.addEventListener('custome',function(){

        })
        ev.dispatchEvent(eve)//触发事件
        CustomEvent可以给事件加数据 
