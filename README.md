# OnlineBookstore
An Online Bookstore implemented in Java that provides a platform for seller and buyer to trade.<br>
一个用Java实现的买卖家在线交易书籍的网上书店。

## Screenshot
![](http://yaochenkun.cn/wordpress/wp-content/uploads/2016/07/shucong1.png)
![](http://yaochenkun.cn/wordpress/wp-content/uploads/2016/07/shucong5.png)
![](http://yaochenkun.cn/wordpress/wp-content/uploads/2016/07/shucong6.png)
![](http://yaochenkun.cn/wordpress/wp-content/uploads/2016/07/shucong9.png)

## Environment
1. Java: __JDK 1.7.0_79__
2. Server: __Jetty 8__
3. Database: __MySQL 5.1__
4. IDE: __eclipse-jee-mars__

## Deployment
One way to depoly this program is just to put Directory [OnlineBookstore](https://github.com/yaochenkun/OnlineBookstore/tree/master/OnlineBookstore) into webapp in Tomcat's or Jetty's Directory, while the other way is for debugging:
### MySQL
1. setup MySQL 5.1 and start MySQL service;
2. create a database named 'online_bookstore' and run [online_bookstore.sql](https://github.com/yaochenkun/OnlineBookstore/blob/master/online_bookstore.sql) to import data;
3. if you want to change the username and password of database, you can rewrite them in OperDB.java.

### Project
1. import [OnlineBookstore](https://github.com/yaochenkun/OnlineBookstore/tree/master/OnlineBookstore) into IDE;
2. select the JDK bin's installing path for the project while not using JRE;

### Server
1. install Jetty plugin in eclipse;
2. right click the project and click Run As -> Run Jetty. __Be careful that Jetty's version should be '8.x.x', or annotations of WebServlet would not work and servlets' path cannot be found.__
3. you can also change the port and the context of this project(server) in Run As -> Run Configuration.

## Key Points
* use simple __Java Servlet__ to get/forward request and send response.
* use __MVC pattern__ to decouple View(JSP) from Controller(XXXClServlet) and Model(XXXBeanCl and XXXBean).
* create __6 key tables__ to undertake the tasks of all the bussinesses.For details you can reach [online_bookstore.sql](https://github.com/yaochenkun/OnlineBookstore/blob/master/online_bookstore.sql).

## For More
If you want to learn more about the development of this project, you can visit [网上书店简介.pdf](https://github.com/yaochenkun/OnlineBookstore/blob/master/网上书店简介.pdf) and [网上书店开发文档.pdf](https://github.com/yaochenkun/OnlineBookstore/blob/master/网上书店开发文档.pdf).
