# flexgw
Flex GateWay 本程序提供了VPN、SNAT、IPSec VPN 基础服务
操作系统 Centos 6.x
解决点击 拨号vpn出现服务器内部错误问题

修改/usr/local/flexgw/website/vpn/dial/services.py
250行:
datetime.strptime(status['ct'],'%c')


解决生成证书错误问题
修改/usr/local/flexgw/scripts/cert-build
52行增加:echo "01" > /usr/local/flexgw/scripts/keys/serial
