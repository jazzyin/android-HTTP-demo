android-HTTP-demo
======
A simple demo for android login and register with MySQL via HTTP(TomCat).


<img src="/1.png" width="250">
<img src="/2.png" width="250">

 Environment
-----
Eclipse + TomCat + MySQL +(Adnroid Studio)

 Usage
-----
Set up MySQL
 - ```create database test;```
 - ```use test;```
 - ```CREATE TABLE `student` (`id` int(11) NOT NULL AUTO_INCREMENT,`username` varchar(20) NOT NULL,`password` varchar(20) NOT NULL,PRIMARY KEY (`id`)) ENGINE=InnoDB AUTO_INCREMENT=30 DEFAULT CHARSET=utf8;```
	
	
Set up TomCat Server
 - In \HelloWeb\src\com\db\DBManager.java ， change ```MySQL-USER``` and ```MySQL-PASS```to your own MySQL username and password.

 
Set up Android demo(there are two version demo for  Android Studio(AS) and Eclipse, you can choose one by your IDE).
 - In \AndroidHTTPDemo\app\src\main\java\com\jazzyin\web\WebService.java, change ```TOMCATURL``` to your own TomCat IP.

 
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
