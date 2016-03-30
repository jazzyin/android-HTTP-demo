android-HTTP-demo
======
A simple demo for android login and register with MySQL by TomCat.

一个使用TomCat使android客户端与mySQL进行注册、登陆等数据交互的demo。

<img src="/1.png" width="250">
<img src="/2.png" width="250">

 Usage
-----
Set up MySQL
配置MySQL
 - ```create database test;```
 - ```use test;```
 - ```  TABLE `student` (`id` int(11) NOT NULL AUTO_INCREMENT,`username` varchar(20) NOT NULL,`password` varchar(20) NOT NULL,PRIMARY KEY (`id`)) ENGINE=InnoDB AUTO_INCREMENT=30 DEFAULT CHARSET=utf8;```
	
	
Set up TomCat Server
配置Tomcat服务器
 - In \HelloWeb\src\com\db\DBManager.java ， change ```MySQL-USER``` and ```MySQL-PASS```to your own MySQL username and password.
 - 打开 \HelloWeb\src\com\db\DBManager.java ， 把 ```MySQL-USER``` 和 ```MySQL-PASS``` 改为你自己MySQL数据库的账号和密码。

 
Set up Android demo(there are two version demo for  Android Studio(AS) and Eclipse, you can choose one by your IDE).
配置Android客户端(此处有两个版本的demo，分别是AS版和Eclipse，可以根据自己的编译器版本选择)。
 - In \AndroidHTTPDemo\app\src\main\java\com\jazzyin\web\WebService.java, change ```TOMCATURL``` to your own TomCat IP.
 - 在 \AndroidHTTPDemo\app\src\main\java\com\jazzyin\web\WebService.java中， 把```TOMCATURL```改为你自己的TomCat服务器IP。
 
 Reference
-----
 http://www.cnblogs.com/yzxk/p/4749440.html
 
 License
-------
    Copyright 2016 jazzyin

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
