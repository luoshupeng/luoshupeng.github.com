---
title: Spring Boot 2.0 多数据源编程
date: 2019-03-19 14:21:31
tags: Spring Boot
categories: Spring Boot
---
# Spring Boot 2.0 多数据源编程

在Spring Boot 1.5.x之前，多数据源编程已经有很多教程和例子了，比如[恒宇少年的博客](https://www.jianshu.com/p/9f812e651319)还有[程序猿DD的博客](http://blog.didispace.com/springbootmultidatasource/)，我就是在两位大拿的教程下学习的。  

但是在升级到Spring Boot 2.0后，一些配置及用法有了变化，如果不小心就会碰到“jdbcUrl is required with driverClassName.”的错误，详细错误信息可以查看[这里](https://www.oschina.net/question/221134_2275771)。  

我经过一番努力，查找资料，终于找到了解决办法，在这里分享出来，省得后来者再去查找资料。  

第一种方法：  
在配置文件中使用spring.datasource.jdbc-url，而不是通常使用的spring.datasource.url。
![输入图片说明](https://static.oschina.net/uploads/img/201803/20153845_U7aE.png "在这里输入图片标题")  
**在这里也请大佬们帮忙解释下spring.datasource.jdbc-url和spring.datasource.url的区别。**  

第二种方法：  
在数据源配置时使用DataSourceProperties方法。  
![输入图片说明](https://static.oschina.net/uploads/img/201803/20154124_5Gos.png "在这里输入图片标题")  

最后，我的微信号是chinesedragon，二维码在最后，欢迎朋友们共同学习。  


[GITEE源码https://gitee.com/shupengluo/SpringBoot2.0-MultiDataSource](https://gitee.com/shupengluo/SpringBoot2.0-MultiDataSource)  
[GITHUB源码https://github.com/luoshupeng/SpringBoot2.0-MultiDataSource](https://github.com/luoshupeng/SpringBoot2.0-MultiDataSource)  

[**参考资料https://docs.spring.io/spring-boot/docs/2.0.0.RELEASE/reference/htmlsingle/#howto-two-datasources**](https://docs.spring.io/spring-boot/docs/2.0.0.RELEASE/reference/htmlsingle/#howto-two-datasources)  

![输入图片说明](https://static.oschina.net/uploads/img/201803/20154840_c2bk.jpg "在这里输入图片标题")