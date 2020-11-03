# README

```sql
-- 创建数据库
create database test;
-- 创建用户
create user test@'%' identified by 'test0755';

-- 修改用户密码
-- grant all privileges on test.* to test@% identified by 'chpass';  

-- 授予用户test管理test的全部权限
-- grant select,insert,update,delete
grant all privileges on test.* to test;

-- 刷新
flush privileges;
```