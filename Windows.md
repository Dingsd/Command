## 微信多开bat文件
````
@echo "Start WeChat"
cd "C:\Program Files (x86)\Tencent\WeChat\"
start WeChat.exe
start WeChat.exe
exit
````
网络上还有其他命令代码，我目前使用的这种，总体来原理一样，通过bat文件的cmd命令启动微信，微信启动路径需要换成实际安装路径；
当然，直接将bat文件放在微信的安装目录下，可以不需要`cd "C:\Program Files (x86)\Tencent\WeChat\"`命令。