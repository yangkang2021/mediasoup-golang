# SMS Server GO
> 这是一个对mediasoup worker的golang封装

## 【单进程】架构模式
1. 用cgo，启动N个mediasoup-worker协程。
2. go使用mediasoup-worker静态库，编译后单文件运行
3. 实现零配置启动
4. 自动获取内外网ip，实现内网同时提供服务。
5. 支持守护进程，挂掉重启。
6. 支持windows、linux、mac上运行。
7. 作为微服务加入到mediasoup的集群
