CentOS最小化安装（版本CentOS7.6）
------
##### 安装扩展源epel
    yum install epel-release 安装扩展源
    yum update 更新系统
##### 安装X Window system
    yum groupinstall "X Window system"
##### 安装Xfce
    yum groupinstall xfce
    systemctl isolate graphical.target 进入xfce界面
##### 设置默认启动图形界面
    systemctl set-default graphical.target
##### 常用工具
    yum install file-roller 归档管理器（解压缩）
    yum install bash-completion 终端自动补全
    yum install gedit.x86_64 文本编辑器
    yum install firefox.x86_64 firefox浏览器64位，32位为firefox.i686
    yum install seahorse.x86_64 密码和密钥
##### 端口监听
    sudo /usr/sbin/tcpdump -s 0 -X 'tcp dst port 21579'