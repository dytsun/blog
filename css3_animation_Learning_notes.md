## css3 animation Learning notes

### CSS3 transition 属性

定义和用法
> transition 属性是一个简写属性，用于设置四个过渡属性：
> transition: property duration timing-function delay;

*  transition-property    规定设置过渡效果的 CSS 属性的名称。(值：none, all, propety)
*  transition-duration    	规定完成过渡效果需要多少秒或毫秒。(值：5s)
*  transition-timing-function    	规定速度效果的速度曲线。(值：linear匀速, ease慢快慢, ease-in慢速开始, ease-out慢速结束,ease-in-out慢速开始和结束, 
   cubic-bezier(n, n, n, n) )在 cubic-bezier 函数中定义自己的值。可能的值是 0 至 1 之间的数值。)
*  transition-delay   	定义过渡效果何时开始。
