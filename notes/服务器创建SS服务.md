来源：http://blog.sina.com.cn/s/blog_16a3cb7cb0102xbvd.html

SSR脚本安装正式开始
等到出现root@host~字样，
复制下面脚本第1条命令，回车：
脚本命令1

wget --no-check-certificate -O shadowsocks-all.sh https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocks-all.sh
（备注：国外服务器运行脚本时容易出错，如出现错误提示 bash: wget: command not found，可以请在先执行 yum -y install wget 命令。成功后，再执行上面的命令。如果没有出现提示错误，请略过）



等出现了上图显示后，输入第2条脚本命令，回车：

脚本命令2

chmod +x shadowsocks-all.sh

等出现了上图显示后，输入第3条脚本命令，回车：

脚本命令3

./shadowsocks-all.sh 2>&1 | tee shadowsocks-all.log
 出现以上画面，根据需要选择，不懂的话直接选1，或者默认回车
下面会提示你输入你的SS SERVER的密码，和端口。不输入就是默认。跑完命令后会出来你的SS客户端的信息。手把手教你vps搭建属于自己的ss教程，开始科学上网吧（本文利用vultr171014更新 <wbr><wbr><wbr>youtube1080p无压力）

手把手教你vps搭建属于自己的ss教程，开始科学上网吧（本文利用vultr171014更新 <wbr><wbr><wbr>youtube1080p无压力）
输入后，回车！

 特别注意，由于iphone端的的wingy目前只支持到cfb，所以我们选择aes-256-cfb，即7 ，回车

这一步按回车继续
然后需要几分钟的安装过程，请耐心等待出现下面的画面！


请立即copy下来加以保存。

上面的命令全部回车执行后，如果没有报错，即为执行成功，出现确认提示的时候，输入 y 后，回车即可。
安装完成后，脚本提示如下：
Congratulations, Shadowsocks-Python server install completed!
Your Server IP : IP地址
Your Server Port : 端口
Your Password : 密码
Your Encryption Method: aes-256-gcm

Your QR Code: (For Shadowsocks Windows, OSX, Android and iOS clients)
ss://YWVzLTsadsa206YnVkZHkyMDA4QDEwNC4yMjQuMTM1Ldfghdfgk=
Your QR Code has been saved as a PNG file path:
/root/shadowsocks_python_qr.png

Welcome to visit: https://teddysun.com/486.html
Enjoy it!

记录保存好你的上述信息：Server IP、Server Port、Password、Encryption Method
这时你的专属ss已经大好了，开始使用吧。
