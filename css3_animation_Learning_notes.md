## css3 animation Learning notes

### CSS3 transition 属性

#### 定义和用法

**transition 属性是一个简写属性，用于设置四个过渡属性：**

**transition: property duration timing-function delay;**

*  transition-property    规定设置过渡效果的 CSS 属性的名称。(值：none, all, propety)
 
*  transition-duration    	规定完成过渡效果需要多少秒或毫秒。(值：5s)

*  transition-timing-function    	规定速度效果的速度曲线。(值：linear匀速, ease慢快慢, ease-in慢速开始, ease-out慢速结束, ease-in-out慢速开始和结束, cubic-bezier(n, n, n, n) )在 cubic-bezier 函数中定义自己的值。可能的值是 0 至 1 之间的数值。)

*  transition-delay   	定义过渡效果何时开始。(值：2s)

### CSS3 animation 属性

#### 定义和语法

**animation 属性是一个简写属性，用于设置六个动画属性;**

**animation: name duration timing-function delay iteration-count direction;**

* animation-name    规定需要绑定到选择器的 keyframe 名称。(值：keyframename|none)

* animation-duration    规定完成动画所花费的时间，以秒或毫秒计。(值：2s)

* animation-timing-function    规定动画的速度曲线。(值：linear匀速, ease慢快慢, ease-in慢速开始, ease-out慢速结束, ease-in-out慢速开始和结束, cubic-bezier(n, n, n, n) )在 cubic-bezier 函数中定义自己的值。可能的值是 0 至 1 之间的数值。)

* animation-delay    规定在动画开始之前的延迟。(值：2s)

* animation-iteration-count    规定动画应该播放的次数。(值：1或infinite)

* animation-direction     规定是否应该轮流反向播放动画。(值：normal和alternate轮流反向播放)


