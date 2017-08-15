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

sudo easy_install pip  
