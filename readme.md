# cmd background
start /b npm start

# install express.js using node.js
npm install express -g


# log into mysql on linux  
mysql -uroot --password='London123!'

# change mysql password
update user set authentication_string=password("London123!") where user='root';



# create mysql user
CREATE USER 'mysql'@'localhost' IDENTIFIED BY 'MyNewPass4!';  
CREATE USER 'mysql'@'114.94.95.222' IDENTIFIED BY 'MyNewPass4!';  


update user set authentication_string=password("MyNewPass4!") where user='mysql';  
select * from mysql.user;  
mysql -umysql -p  

# grant privileges to a user
GRANT ALL ON boardgames.bggdata TO 'mysql'@'localhost';  

GRANT ALL ON boardgames.* TO 'mysql'@'114.94.95.222';  
GRANT ALL ON boardgames.* TO 'root'@'114.94.95.222';

CREATE USER 'mysql'@'%' IDENTIFIED BY 'MyNewPass4!';  
GRANT ALL ON boardgames.* TO 'mysql'@'%';  

sudo easy_install pip  

# install packages
pip install mysql-connector==2.1.6

# pip mirror
Linux下，修改 ~/.pip/pip.conf (没有就创建一个)， 修改 index-url至tuna，内容如下：  
 
 [global]  
 index-url = https://pypi.tuna.tsinghua.edu.cn/simple  
 
清华: https://pypi.tuna.tsinghua.edu.cn/simple  
豆瓣: http://pypi.douban.com/simple/  
阿里: http://mirrors.aliyun.com/pypi/simple/  
