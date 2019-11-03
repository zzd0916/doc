# linux 命令大全

## 重要命令
#### 行编辑器 vi/vim
- cmd: vi 文件名 （首次进入为命令模式，通过输入命令进行编辑操作）
- 输入i/a：进入插入模式
- 按esc回到命令模式   
- 保存并退出 :wq enter
- 不保存退出 :q!  enter
- 退出 :q enter
- 搜索 /检索词 enter  向下查找输入n, 向上查找shift+n,还可配置检索此高亮显示

#### 服务管理命令 systemctl

#### 网络管理命令 ifconfig、ip命令、router
- ifconfig (windows下ipconfig) 显示当前机器的网络配置

#### 命令行下载命令 curl wget
##### wget
- 下载文件: wget 下载地址 
- wget查看帮助: wget --help  
- wget查看详细文档说明： man wget
##### curl
- 下载文件: curl 下载地址 -o 要取的文件名
- wget查看帮助: wget --help  
- wget查看详细文档说明： man wget

#### 怎么查看linux帮助

#### 在终端下不小心 ctrl+s 怎么办
ctrl+s 会挂载终端（暂停屏幕输出）
使用 ctrl+q : 恢复屏幕输出

##### 常用终端快捷键
- ctrl+c : 结束正在运行的程序【ping、telnet】
- ctrl+d : 结束输入或退出shell
- ctrl+s : 暂停屏幕输出
- ctrl+q : 恢复屏幕输出
- ctrl+l : 清屏，等同于clear命令
- ctrl+a/ctrl+e : 快速移动光标到开头/结尾
- esc + backspace: 快速删除当前输入命令

#### 进程管理相关命令
进程： 进程的目的就是担当分配系统资源（CPU，内存）的实体
线程： 线程是操作系统能进行运算调度的最小单位
协程： 协程是一种用户态的轻量级线程，无法利用多核资源
IO密集型应用发展： 多进程->多线程->事件驱动->协程
CPU密集型应用的发展：多进程->多线程
调度和切换的时间：进程->线程->协程


- top命令
- ps命令
- kill、pkill命令使用及注意事项
- w命令



## 基础命令
- 列出当前目录: ls 或者是 dir
- 列出当前目录及详细信息: ls -l (权限，文件数量，当前文件属于哪个用户组和用户，大小，创建时间，目录名称)
- 显示隐藏文件: ls -a
- 进入文件夹: cd project-name
- 返回上一层: cd ..
- 回到当前用户目录: cd ~
- 回到根目录: cd /  
- 创建文件夹: mkdir name -p (-p为可选，创建多级目录需要用到)
- 复制文件: cp 文件名 放置的路径/新名称
- 复制目录: cp -R 文件名 新名称
- 删除文件: rm 文件名
- 删除目录: rm -r 目录名
- 查看当前目录路径: pwd
- 关机： shutdown now -h
