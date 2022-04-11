####mysql install

```
# mysql 설치
$ sudo dnf search mysql
$ sudo dnf install mysql-server .x86_64 -y
$ sudo systemctl start mysqld
```

```

# 유저 만들기
$ sudo mysql -u root
mysql> alter user root@localhost identified by '1234';
mysql> flush privileges;	(새로고침)

# 접속 하기
$ mysql -u root -p1234	(유저는 띄어쓰기, 패스워드는 붙여쓰기)
$ sudo mysql -u root -p	(보안접속)

# 계정 만들기
mysql> create user user01@localhost identified by '1234';
mysql> flush privileges;
mysql> create user 'user01'@'%' identified by '1234';
mysql> flush privileges;

# 권한 주기
mysql> grant all privileges on *.* to 'user01'@'localhost';
mysql> flush privileges;
```

```
# 데이터 베이스 목록 확인
mysql> SHOW DATABASES;

# 데이터 베이스 선택
mysql> USE `test01`;

# 테이블 생성
mysql> CREATE TABLE `test_table02` (
	`num` INT NULL,
	`name` VARCHAR(50) NULL DEFAULT NULL
)
COLLATE='utf8_general_ci';

# 테이블 내용 확인
mysql> SELECT * FROM `test01`.`test_table02` LIMIT 1000;

# 테이블 데이터 입력
mysql> INSERT INTO `test01`.`test_table02` (`num`, `name`) VALUES ('1111', 'aaa');
```

<pre>

oracle
	./oracle		(설치파일)
	sqlplus		(실행파일)
	
mysql & maraiDB
	mysqld		(설치파일)
	mysql		(실행파일)
	
mongoDB
	mongod		(설치파일)
	mongo		(실행파일)
</pre>
	