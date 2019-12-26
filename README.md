1. 记得看打印日志 的router信息路径
2019-12-26 13:27:57.602  INFO 44064 --- [ : Mapped "{[/login/to_login]}" onto public java.lang.String 
2. 导出表结构和数据
3.修改端口
在application.properties 增加一行 server.port=8084
4.给增加的表添加初始用户数据
 此类可以使用 com.imooc.miaosha.util.UserUtil
 5. 增加秒杀商品内容
 http://localhost:8084/goods/to_detail2/1  进入没有验证码的页面
http://localhost:8084/goods_detail.htm?goodsId=2  进入有验证码的页面
6. 订单详情一个 用ajax实现  一个用 spring模板页面实现
7.订单已产生地址：http://localhost:8084/order_detail.htm?orderId=0