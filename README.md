phpcms_postgres
===============

phpcms postgresql db adapter
phpcms的postgresql数据库支持功能。

由于phpcms原生程序对数据库广泛支持的细节考虑还不是很完善，所以在支持postgresql的时候做了适当的修改以适应，具体修改的几点如下：

- mysql中数据表、字段名等为了防止与关键字冲突需要用符号“`”括起来，而postgresql中却是用的双引号来标志，phpcms中的model.php文件里面直接用了mysql的方法
- mysql中limit的写法以及 postgresql中limit offset写法不同的问题
- mysql自增序列获取与postgresql中自增序列获取的问题处理


