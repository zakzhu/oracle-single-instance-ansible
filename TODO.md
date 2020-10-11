# 接下来需要做的

- 完善 oracle_env role

- sqlplus pretty output 配置, 以及考虑 sqlcl 工具

- common role 执行每个 rsp file 后, 增加 debug 输出 stdout 和 stderr

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

-
