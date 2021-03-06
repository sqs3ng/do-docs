---
title: do_Alipay 组件
---

### <SPAN style="TEXT-DECORATION: line-through">do_Alipay 组件</SPAN>(已废弃,请使用do_Alipay1)

 支持平台: iOS7.0,Android4.0 以上
 [组件示例](https://github.com/do-api/docs-example/tree/master/source/view/do_Alipay)
 调用手机支付宝客户端，完成支付功能

#### <font color ='#40A977'>**0.**</font> 目录

     | ID | 说明
---- |------|------|
<font color ='#0092db'>异步方法</font>  |[pay](#pay)| 支付

#### <font color ='#40A977'>**1.**</font> 属性

#### <font color ='#40A977'>**2.**</font> 同步方法

#### <font color ='#40A977'>**3.**</font> 异步方法

>##### <span id=pay><font color ='#0092db'>**pay**</font></span>: 支付

- 参数:

  名称 | 类型 |必填|默认值|说明
  ---- |-------------  |--------------|--------|------
  **rsaPrivate** |<font color ='#808000'>**string**</font> | 是 | |通过支付宝提供的工具生成的
  **rsaPublic** |<font color ='#808000'>**string**</font> | 是 | |通过支付宝提供的工具生成一个用户公钥，然后上传到支付宝网站，返回一个支付宝公钥
  **partner** |<font color ='#808000'>**string**</font> | 是 | |签约的支付宝账号对应的支付宝唯一用户号。以2088开头的16位纯数字组成。
  **notifyUrl** |<font color ='#808000'>**string**</font> | 是 | |支付宝服务器把处理结果返回该url，长度不能超过200个字符
  **tradeNo** |<font color ='#808000'>**string**</font> | 是 | |支付宝合作商户网站唯一订单号,长度不能超过64个字符
  **subject** |<font color ='#808000'>**string**</font> | 是 | |商品的标题/交易标题/订单标题/订单关键字等,长度不能超过128个字符
  **sellerId** |<font color ='#808000'>**string**</font> | 是 | |卖家支付宝账号（邮箱或手机号码格式）或其对应的支付宝唯一用户号,长度不能超过16个字符
  **totalFee** |<font color ='#808000'>**string**</font> | 是 | |该笔订单的资金总额，单位为RMB-Yuan。取值范围为[0.01，100000000.00]，精确到小数点后两位。
  **body** |<font color ='#808000'>**string**</font> | 是 | |对一笔交易的具体描述信息。如果是多种商品，请将商品描述字符串累加传给body,长度不能超过512个字符。
  **timeOut** |<font color ='#808000'>**string**</font> | 否 | |设置未付款交易的超时时间，一旦超时，该笔交易就会自动被关闭。
当用户输入支付密码、点击确认付款后（即创建支付宝交易后）开始计时。
取值范围：1m～15d，或者使用绝对时间（示例格式：2014-06-13 16:00:00）。
m-分钟，h-小时，d-天，1c-当天（无论交易何时创建，都在0点关闭）。
该参数数值不接受小数点，如1.5h，可转换为90m。
- 返回值类型 : <font color ='#808000'>**object**</font>
- 返回值描述: {'code':'9000','msg':'success'}，其中code的9000为订单支付成功,8000为正在处理中,4000为 订单支付失败,6001为用户中途取消,6002为网络连接出错
- 说明: 调用支付宝支付
- 示例:

  ```javascript
  ...

  ```

[回到顶部](#top)


#### <font color ='#40A977'>**4.**</font> 事件
