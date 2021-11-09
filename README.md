	# 1.Linux入门不是要学“Linux”

1.1.1体验：比较和其他系统的不同和相同点

2.Linux GUI->Shell

四大组成部分：
1.Linux 内核（kernel）
2.GNU工具
3.GUI desktop环境
4.application应用
GNU/Linux
Linux的内核组成：GUI和GNU

Linux的内核组成：
3.系统内存
4.文件管理

文件系统：读和写的标准

GNU组织
1.GNU核心：
原本在Unix上的一些命令移植到了Linux上。
供Linux使用的这套工具：coreutils coreutilitle软件包

（1）用来处理文件的工具
（2）用来操作文本的工具
（3）用了管理进程的工具
2.Shell提供给用户使用的软件：用户拿它来使用电脑，并且和电脑交互

纯命令的界面给用户使用（CLI）;
图层给用户使用（GUI）.

Linux shell —>CLI

命令：
bash shell基础shell

keith@keith-virtual-machine:~$

用户名@机器名：当前所在目录

~    当前用户目录

$    等待用户输入

第三方的shell

shell命令：

man ls：知道命令的意思文档。

page dowm和page up上下翻阅。

www.wangchujiang.com。

白色的是文件，蓝色的是文件夹。

clear清屏

ctrl+u清格

ls：用来显示文件

ls -a：显示带.的文件

ls -al：列出所有文件（包括隐藏的）详细信息

ls -hl：列出文件的大小

ll ：按用户进行分类

cd ..返回上一目录。

Linux的根目录：
区别windows；
windows盘符。
解析：
/home 用户配置目录
/etc  系统配置文件目录
/lib  库目录
/lost+found
/mnt 挂载目录
/proc 伪装目录
/run  运行目录
/tmp  临时目录
/var  经常变化的目录 ：日志
/boot 启动目录
/dev  设备目录：设备管理器
/opt  第三方软件目录
/root 管理员目录、root目录和用户目录分开

sudo rm-rf/*删库命令
/sbin 高级管理员目录
/stv  服务目录 本地服务
/usr  用户二进制目录

cd命令：切换用户当前目录
CTRL +C暂停
CTRL+ shift+c 复制，粘贴v

文件目录：
我在那？相对于谁
1.绝对路径(全)
一层一层，和快递地址一样
2.相对路径（不全）
单点符，当前文件夹
双点符，当前目录的父目录

和ls有关的命令：
-F 区分文件夹和文件}
-R	遍历	   }->FR

TOUCH命令：更新时间，创建一个新的文件
cp命令：CP 你想复制的文件（）？你想复制到哪（）？
cp -i命令，提醒用户

常用的小技巧：
tab键制表符
CTRL +方向键，左右跳跃
CTRL+A,开头，CTRL+E,结尾

.link：
链接文件、
1.符号链接（软链接）——快捷方式
原来文件/文件夹必须存在
2.硬链接：
创建副本
原来的文件/文件夹必须存在

更上一层的shell：
如何用命令：
ps axo pid,comm,pcpu #查看进程的PID、名称以及CPU占用率
ps -aux |grep namd #查看named进程详细信息
任务管理器



父子shell：
dash



vim：
1.sudo apt install vim
2.编辑模式——>普通模式
insert——i
退出 esc

保存
:wq；
w：write
q：quit

vim 文件名	进
cat 文件名	看
h：向左
j：向上
k：向下
L：向右

Ctrl B 向上	Ctrl E 向上
Ctrl F 向下	Ctrl Y 向下


shift G 最后一行
gg  最开始

:q! 都不保存

不同方式的插入编辑文本，
i 光标前插入
a 光标后插入
o 直接enter到下一行输入
x 删除光标所在字符
dd 删除整个一行
u 撤销
dw 移除当前光标所在的单词。
跳跃光标
b	跳跃单词首字母
e	跳跃单词最后
w	先跳跃到首字母再跳到最后
shift 联合操作

shift +6 跳跃到本行的开头
shift +4 跳跃到本行的末尾




vim的复制粘贴：
yw:复制一个单词
y$：复制光标到末尾

p：粘贴

008.安装软件

apt install 安装

sudo apt update：相当于查找更新

sudo apt upgrade：相当于一键更新

sudo apt remove:卸载

安装别的软件：

apt里安装不了的软件
