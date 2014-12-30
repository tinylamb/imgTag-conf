### imgTag 程序配置

#### 1 系统环境

* 64位 Ubuntu

* Qt creator

#### 2 依赖包

1. libxml2

   ```
   sudo apt-get install libxml2
   sudo apt-get install libxml2-dev
   dpkg -L libxml2-dev #查看安装信息

   ```
   
2. libcurl

   `sudo apt-get install curl`
   
   
3. Flickcurl

	见[Flickcurl: C library for the Flickr API](http://librdf.org/flickcurl/)

4. opencv

	见[jayrambhia/Install-OpenCV](https://github.com/jayrambhia/Install-OpenCV)
	
	下载Install-OpenCV/Ubuntu/2.4/opencv2_4_9.sh 
	
	执行`chmod +x opencv2_4_9.sh;./opencv2_4_9.sh`

5. mysql

	```
	sudo apt-get install mysql-server
	sudo apt-get install mysql-client
	sudo apt-get install libmysqlclient-dev
	sudo netstat -tap | grep mysql #socket 处于listen状态则安装成功
	mysql -u root -p #登陆
	
	```
	如果登陆失败
	
	cat /etc/mysql/debian.cnf
	
	找到 user , password 信息
	
	mysql -u USER -p
	
	输入 PASSWORD 进入mysql
	
	SET PASSWORD FOR 'root'@'localhost' = PASSWORD('NEWPASSWORD');
	
	flush privileges;
	
	quit;
	
	用新密码登陆 mysql -u root -p

6. mysql++

	`sudo apt-get install libmysqlclient-dev libmysqld-dev libmysql++-dev libmysql++-doc libmysql++3
`

	This will install the mysql head files in /usr/include/mysql ;
	
	mysql++ head files in /usr/include/mysql ;
	
	libmysqlpp.so and libmysqlclient.so in /usr/lib. 
