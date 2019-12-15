我们有时会纠结是BBR速度更快还是锐速更快，安装的时候也要分别找脚本，但是loc的大佬做了个集合了BBR原版、BBR魔改、BBR Plus和锐速的脚本，想用哪个用哪个，很方便！

在vultr上Centos 7, Debian 8/9, Ubuntu 16/18测试通过。不支持OVZ和LXC。

建议SSH下，root用户。

一、安装证书

apt-get -y install ca-certificates或yum -y install ca-certificates

二、安装 wget "https://raw.githubusercontent.com/cherry90060/Linux-NetSpeed/master/tcp.sh" && chmod +x tcp.sh && ./tcp.sh


1、先在[1 – 3]切换内核（第一次显示为bbr内核也要切换一遍），重启

BBR原版/BBR魔改/BBR plus/锐速 四合一脚本

出现内核切换的这个选no

BBR原版/BBR魔改/BBR plus/锐速 四合一脚本

2、重启后不用再下载脚本，直接 ./tcp.sh ，在[4 – 8]中选你要开的加速

“1. 安装 BBR/BBR魔改版内核” 对应4,5,6（原版，魔改，暴力魔改）
“2. 安装 BBRplus版内核 ” 对应7（plus）
“3. 安装 Lotserver(锐速)内核” 对应8（锐速）

3、开启后输入 命令/root./tcp.sh即可打开脚本 

现在你可以自由的切换你想要的加速，直到你不想折腾为止~
