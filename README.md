

# 使用说明：

进入下载脚本的目录并运行脚本：

``` bash
# 客户端管理菜单
./status.sh c
# 服务端管理菜单
./status.sh s
```

然后选择你要执行的选项即可。

``` bash
ServerStatus 一键安装管理脚本 [vx.x.x]
-- Toyo | doub.io/shell-jc3 --
 
0. 升级脚本
————————————
1. 安装 服务端
2. 卸载 服务端
————————————
3. 启动 服务端
4. 停止 服务端
5. 重启 服务端
————————————
6. 设置 服务端配置
7. 查看 服务端信息
8. 查看 服务端日志
————————————
9. 切换为 客户端菜单
 
当前状态: 服务端 已安装 并 已启动
 
请输入数字 [0-9]:
```
# 其他操作

### 客户端：

启动：service status-client start

停止：service status-client stop

重启：service status-client restart

查看状态：service status-client status

### 服务端：

启动：service status-server start

停止：service status-server stop

重启：service status-server restart

查看状态：service status-server status

### Caddy（HTTP服务）：

启动：service caddy start

停止：service caddy stop

重启：service caddy restart

查看状态：service caddy status

Caddy配置文件：/usr/local/caddy/caddy



——————————————————————————————————————

安装目录：/usr/local/ServerStatus

网页文件：/usr/local/ServerStatus/web

配置文件：/usr/local/ServerStatus/server/config.json

客户端查看日志：tail -f tmp/serverstatus_client.log

服务端查看日志：tail -f /tmp/serverstatus_server.log

# 其他说明

网络实时流量单位为：G=GB/s，M=MB/s，K=KB/s

服务器总流量单位为：T=TB，G=GB，M=MB，K=KB

### CentOS7系统 负载显示异常的问题

CentOS7系统 默认可能没有安装 netstat 依赖，所以会造成IP检测(负载)出错，手动安装即可：
`yum install net-tools -y `

# 相关开源项目，感谢： 

* ServerStatus：https://github.com/BotoX/ServerStatus
* mojeda: https://github.com/mojeda 
* mojeda's ServerStatus: https://github.com/mojeda/ServerStatus
* BlueVM's project: http://www.lowendtalk.com/discussion/comment/169690#Comment_169690
