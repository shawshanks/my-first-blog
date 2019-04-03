# my-first-blog

## 项目背景
来自于GitBook中的一个项目: [Django博客入门](https://www.gitbook.com/book/shenxgan/django/details)

## 项目中遇到的坑
### 1.MySQLdb安装
问题:使用`pip3 install mysql-python`命令安装时, 一直出现`ImportError: No module named 'ConfigParser'`错误. 将依赖包安装完成后, 还是不行. 

原因: 
> In Python 3, ConfigParser has been renamed to configparser for PEP 8 compliance. It looks like the package you are installing does not support Python 3.

解决方法: 
> You can instead use the mysqlclient package as a drop-in replacement for MySQL-python. It is a fork of MySQL-python with added support for Python 3.

[参考链接](http://stackoverflow.com/questions/14087598/python-3-importerror-no-module-named-configparser)
