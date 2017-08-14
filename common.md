# log into mysql on linux  
mysql -uroot --password='London123!'

# change mysql password
update user set authentication_string=password("London123!") where user='root';



# create mysql user
CREATE USER 'mysql'@'localhost' IDENTIFIED BY 'MyNewPass4!';
update user set authentication_string=password("MyNewPass4!") where user='mysql';
select * from mysql.user;
mysql -umysql -p
