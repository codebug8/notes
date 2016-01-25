# oracle

## Linux下oracle数据库启动和关闭操作

### 登陆

root登陆之后切换到oracle用户上，输入

    su - oracle

### 连接

在oracle用户下，输入

    sqlplus /nolog

### 使用管理员权限

    输入 connect /as sysdba

### 启动/关闭服务

    输入 startup

### startup参数

不带参数，启动数据库实例并打开数据库，以便用户使用数据库，在多数情况下，使用这种方式!

nomount，只启动数据库实例，但不打开数据库，在你希望创建一个新的数据库时使用，或者在你需要这样的时候使用！

mount，在进行数据库更名的时候采用。这个时候数据库就打开并可以使用了！

### shutdown的参数

```shell
Normal 需要等待所有的用户断开连接
Immediate 等待用户完成当前的语句
Transactional 等待用户完成当前的事务
Abort 不做任何等待，直接关闭数据库
normal 需要在所有连接用户断开后才执行关闭数据库任务，所以有的时候看起来好象命令没有运行一样！在执行这个命令后不允许新的连接
immediate 在用户执行完正在执行的语句后就断开用户连接，并不允许新用户连接。
transactional 在拥护执行完当前事物后断开连接，并不允许新的用户连接数据库。
abort 执行强行断开连接并直接关闭数据库。
```

### 如果是启动服务，要开启监听

    退出sqlplus模式
    输入 lsnrctl start