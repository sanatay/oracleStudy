# oracleStudy
Oracle 查询优化改写读书笔记

第一章
1.查询表结构
desc tableName
2.查找某一列的值为空值
select * from subs where org_id is null;   --需要用is，而不是=
3.replace函数用法
select replace('abcde','a',null) as str from dual;
replace(原字段,原字段要替换的内容,替换为的内容）
4.coalesce函数
select coalesce(c1,c2,c3,c4,c5,c6) as c from v;
查找v表中，c1,c2,c3,c4,c5,c6不为空的第一个值
