# 接下来需要做的

- 完善 oracle_env role
  [About NLS_LANG Parameters](https://docs.oracle.com/html/B10131_02/gblsupp.htm)

- sqlplus pretty output 配置, 以及考虑 sqlcl 工具

- common role 执行每个 rsp file 后, 增加 debug 输出 stdout 和 stderr

- 增加选择 non-cdb 或 cdb 的变量, response_files/templates/dbca.rsp.j2 中 createAsContainerDatabase 的值

- 修改解压目录为 ORACLE_HOME/ https://docs.oracle.com/en/database/oracle/oracle-database/19/ladbi/running-oracle-universal-installer-to-install-oracle-database.html#GUID-DD4800E9-C651-4B08-A6AC-E5ECCC6512B9

-

# 中后期需要做的

- 统一变量取值

- rpm 依赖包精简, 删除无用的 32 位包
  Starting with Oracle Database 11g Release 2 (11.2.0.2),
  **all the 32-bit packages, except for gcc-32bit-4.3**, listed in the following table are no longer required for installing a database on Linux x86-64. Only the 64-bit packages are required.

- 实现 common role 的 idempotent

-

# 大后期需要做的

- 该项目默认会用 dbca 创建一个数据库,
  后续开发单独的 dbca 创建库的自动配置工具

- 以及考虑对应创建监听端口

- 阅读 oracle 数据库调优 doc

- 增加内存扩容后, 数据库调优参数自动相应修改

- 考虑尽可能不修改 grub 定制 boot, 而是通过添加重启后命令修改的计划任务来即时改变 boot 参数

- 添加服务开机自启动
  https://www.zybuluo.com/clisdodo/note/1490389#211-%E6%B7%BB%E5%8A%A0%E5%90%AF%E5%8A%A8%E5%85%B3%E9%97%AD%E6%95%B0%E6%8D%AE%E5%BA%93%E6%9C%8D%E5%8A%A1%E8%84%9A%E6%9C%AC%E5%8F%AF%E9%80%89

- 健康检测

- 删除无用组件的文件

- 完善 post_roles 里的各种 post inst 后的其他操作

- 同时支持 12.2.0.2 和 11.2.0.4 的安装

- clone 工具开发

- 卸载工具开发

-
