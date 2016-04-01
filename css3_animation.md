## css3 animation

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

> 通过规定至少以下两项 CSS3 动画属性，即可将动画绑定到选择器：
> 规定动画的名称
> 规定动画的时长

* animation-name    规定需要绑定到选择器的 keyframe 名称。(值：keyframename|none)

* animation-duration    规定完成动画所花费的时间，以秒或毫秒计。(值：2s)

* animation-timing-function    规定动画的速度曲线。(值：linear匀速, ease慢快慢, ease-in慢速开始, ease-out慢速结束, ease-in-out慢速开始和结束, cubic-bezier(n, n, n, n) )在 cubic-bezier 函数中定义自己的值。可能的值是 0 至 1 之间的数值。)

* animation-delay    规定在动画开始之前的延迟。(值：2s)

* animation-iteration-count    规定动画应该播放的次数。(值：1或infinite)

* animation-direction     规定是否应该轮流反向播放动画。(值：normal和alternate轮流反向播放)

* animation-play-state    规定动画是否正在运行或暂停。(值：running或paused)

* animation-fill-mode    (值：none不改变默认行为；forwards当动画完成后，保持最后一个属性值；backwards在 animation-delay 所指定的一段时间内，在动画显示之前，应用开始属性值；both向前和向后填充模式都被应用)

### CSS3 transform 属性

#### 定义和语法

**transform 属性向元素应用 2D 或 3D 转换。该属性允许我们对元素进行旋转、缩放、移动或倾斜。**

**transform: none|transform-functions;**

*  none    	定义不进行转换。

*  matrix(n,n,n,n,n,n)    		定义 2D 转换，使用六个值的矩阵。

*  translate(x,y)    	定义 2D 转换。
  
*  translateX(x)    定义转换，只是用 X 轴的值。
  
*  translateY(y)    定义转换，只是用 Y 轴的值。
 
*  scale(x,y)    定义 2D 缩放转换。
  
*  scaleX(x)    通过设置 X 轴的值来定义缩放转换。
  
*  scaleZ(z)    	通过设置 Y 轴的值来定义缩放转换。
  
*  rotate(angle)    定义 2D 旋转，在参数中规定角度。
 
*skew(x-angle,y-angle)   	定义沿着 X 和 Y 轴的 2D 倾斜转换。






