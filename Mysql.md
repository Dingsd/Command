Mysql8
------
##### 修改身份认证插件
    alter user 'root'@'localhost' identified with caching_sha2_password by 'root(替换密码)'; 新身份验证插件
    alter user 'root'@'localhost' identified with mysql_native_password by 'root(替换密码)'; 旧身份验证插件
##### 修改初始密码
    grep 'temporary password' /var/log/mysqld.log 执行后会得到一个初始密码