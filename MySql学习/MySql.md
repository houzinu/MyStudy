### Mysql登录方式

-u root -P3306 -h localhsot -p

show variables like 'character_%'---查看预设字符集

show databases;---查看数据库

use ==dbtest==;---进入dbtest数据库

# SELECT基础

select * from tables; // *= 字段，tables=表名

###### 列的别名

Select employee_id ==emp_id==  , last_name ==as== lname , department_id =="==dept_id=="==;

###### 去除重复行

SELECT ==DISTINCT== first_name FROM employees;

![image-20220727172734123](C:\Users\yangc\AppData\Roaming\Typora\typora-user-images\image-20220727172734123.png)

> 所有的null值不参与聚合函数计算。



###### 分组查询

![image-20220728111054120](C:\Users\yangc\AppData\Roaming\Typora\typora-user-images\image-20220728111054120.png)

DQL语句的执行顺序

1.from

2.where

3.groud by , having 

4.select 

5.order by , limit
