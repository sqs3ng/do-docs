---
title: do_GestureView 组件
---

### do_GestureView 组件

 支持平台: iOS7.0,Android4.0 以上
 [组件示例](https://github.com/do-api/docs-example/tree/master/source/view/do_GestureView)
 手势组件，缺省是透明的，windowsPC不支持

#### <font color ='#40A977'>**0.**</font> 目录

     | ID | 说明
---- |------|------|
<font color ='#e96900'>事件</font>  |[touch](#touch)| 按下并在组件范围抬起，触发该事件
<font color ='#e96900'>事件</font>  |[touchDown](#touchDown)| 组件范围内按下即可触发
<font color ='#e96900'>事件</font>  |[touchUp](#touchUp)| 一旦按下，手指离开即触发，不论是否在组件范围内
<font color ='#e96900'>事件</font>  |[longTouch](#longTouch)| 长按触发该事件
<font color ='#e96900'>事件</font>  |[fling](#fling)| 手指在触摸屏上迅速移动，并松开的动作，松开时触发
<font color ='#e96900'>事件</font>  |[move](#move)| 手指在触摸屏上移动时触发

#### <font color ='#40A977'>**1.**</font> 属性

#### <font color ='#40A977'>**2.**</font> 同步方法

#### <font color ='#40A977'>**3.**</font> 异步方法


#### <font color ='#40A977'>**4.**</font> 事件

>###### <span id=touch><font color ='#e96900'>**touch**</font></span>: 按下并在组件范围抬起，触发该事件

- 返回值类型 : <font color ='#808000'>**object**</font>
- 返回值描述: {x:'100',y:'100'} 返回手指在组件内x,y的绝对值
- 说明: 按下并在组件范围抬起，触发该事件
- 示例:

  ```javascript
  ...

  ```

[回到顶部](#top)

>###### <span id=touchDown><font color ='#e96900'>**touchDown**</font></span>: 组件范围内按下即可触发

- 返回值类型 : <font color ='#808000'>**object**</font>
- 返回值描述: {x:'100',y:'100'} 返回手指x,y在屏幕的绝对值
- 说明: 组件范围内按下即可触发
- 示例:

  ```javascript
  ...

  ```

[回到顶部](#top)

>###### <span id=touchUp><font color ='#e96900'>**touchUp**</font></span>: 一旦按下，手指离开即触发，不论是否在组件范围内

- 返回值类型 : <font color ='#808000'>**object**</font>
- 返回值描述: {x:'100',y:'100'} 返回手指x,y在屏幕的绝对值
- 说明: 一旦按下，手指离开即触发，不论是否在组件范围内
- 示例:

  ```javascript
  ...

  ```

[回到顶部](#top)

>###### <span id=longTouch><font color ='#e96900'>**longTouch**</font></span>: 长按触发该事件

- 返回值类型 : <font color ='#808000'>**object**</font>
- 返回值描述: {x:'100',y:'100'} 返回手指x,y在屏幕的绝对值
- 说明: 长按触发该事件
- 示例:

  ```javascript
  ...

  ```

[回到顶部](#top)

>###### <span id=fling><font color ='#e96900'>**fling**</font></span>: 手指在触摸屏上迅速移动，并松开的动作，松开时触发

- 返回值类型 : <font color ='#808000'>**object**</font>
- 返回值描述: {velocityX:'100',velocityY:'100'} 返回手指在手指x,y方向滑动的速率，其中正值表示的是往下和往右、负值表示的是往上和往左。iOS的速率是固定值
- 说明: 手指在触摸屏上迅速移动，并松开的动作，松开时触发
- 示例:

  ```javascript
  ...

  ```

[回到顶部](#top)

>###### <span id=move><font color ='#e96900'>**move**</font></span>: 手指在触摸屏上移动时触发

- 返回值类型 : <font color ='#808000'>**object**</font>
- 返回值描述: {x:'100',y:'100'} 返回手指x,y在屏幕的绝对值
- 说明: 手指在触摸屏上移动时触发
- 示例:

  ```javascript
  ...

  ```

[回到顶部](#top)


