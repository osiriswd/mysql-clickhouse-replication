# mysql-clickhouse-replication

用于从mysql增量同步数据到clickhouse



环境要求：

python 2.7，同时可以利用pypy提高性能。



pypy部署命令

```bash
yum -y install pypy-libs pypy pypy-devel
wget https://bootstrap.pypa.io/get-pip.py
pypy get-pip.py
/usr/lib64/pypy-5.0.1/bin/pip install MySQL-python
/usr/lib64/pypy-5.0.1/bin/pip install mysql-replication
/usr/lib64/pypy-5.0.1/bin/pip install clickhouse-driver
/usr/lib64/pypy-5.0.1/bin/pip install redis
```

如果不使用pypy，而是使用python，那么模块安装命令

```bash
pip install MySQL-python
pip install mysql-replication
pip install clickhouse-driver
pip install redis
```

同步设置参考文档：

https://www.cnblogs.com/gomysql/p/11199856.html