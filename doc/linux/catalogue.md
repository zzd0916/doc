# linux文件系统介绍
linux下，所有的东西都看成文件，其中目录也算一种特殊文件，所以说文件系统可以管理所有的东西。

## 根目录 -- /
进入命令： cd /
相当于进入了windows下： 我的电脑

## bin目录
bin文件夹一般存放命令和脚本
可执行文件没有后缀，脚本后缀为.sh
### 判断是否是可执行文件
使用命令 ： ls -l  后缀带x的就属于可执行文件

## etc目录
一般存入配置文件和重要脚本（千万不要乱操作）

## dev目录
开发用的文件

## home目录
linux为多用户系统, 相当于windows操作系统下的c:/users(用户))目录

## lib,lib64 目录
存放一下系统的库（二进制的库）, 相当于windows操作系统下 c:/windows目录

## mnt,media 目录
计算机上接上u盘或硬盘一般就在media目录下找。
早期linux系统上识别新的存储设备(如u盘)，需要手动敲命令，挂载到mnt目录上。

## proc目录
存储动态数据，系统信息（如Cpu信息）在proc里面，proc文件实际上放在内存中,关机就会消失。
cd proc 
cat cpuinfo 查看cpu信息

## boot目录（千万不要操作）
引导文件，linux内核全在里面。

## opt目录
存放打包好的绿色的软件，相当于 windows系统下的 c:/program files文件夹

## root目录
特殊用户(linux系统管理员)的目录,权限最高

## sbin目录
和bin目录类似

## sys目录
扩展目录


