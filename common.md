# log into mysql on linux  
mysql -uroot --password='London123!'

# change mysql password
update user set authentication_string=password("London123!") where user='root';
