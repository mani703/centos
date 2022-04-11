####my sql install

```
=====mysql 설치=====
$ sudo dnf search mysql
$ sudo dnf install mysql-server .x86_64 -y
$ sudo systemctl start mysqld
```

```

=====유저 만들기=====
$ sudo mysql -u root
mysql> alter user root@localhost identified by '1234';
mysql> flush privileges;	(새로고침)

=====접속 하기=====
$ mysql -u root -p1234	(유저는 띄어쓰기, 패스워드는 붙여쓰기)
$ sudo mysql -u root -p	(보안접속)

=====계정 만들기=====
mysql> create user user01@localhost identified by '1234';
mysql> flush privileges;
mysql> create user 'user01@%' identified by '1234';
mysql> flush privileges;

=====권한 주기=====
mysql> grant all privileges on *.* to 'user01'@'localhost';
mysql> flush privileges;
```

<pre>

oracle
	./oracle	(설치파일)
	sqlplus		(실행파일)
	
mysql & maraiDB
	mysqld		(설치파일)
	mysql		(실행파일)
	
mongoDB
	mongod		(설치파일)
	mongo		(실행파일)
	