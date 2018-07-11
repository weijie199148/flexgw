# flexgw
Flex GateWay 本程序提供了VPN、SNAT、IPSec VPN 基础服务。
解决点击 拨号vpn出现服务器内部错误问题

修改/usr/local/flexgw/website/vpn/dial/services.py
250行:datetime.strptime(status['ct'],'%c')
