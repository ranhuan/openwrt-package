# openwrt-package
openwrt软件包

收集的openwrt软件包，配合官网源码包使用。
尽可能放原作者的仓库地址，自行clong到openwrt源码的package目录，然后在make menuconfig中选中后编译。

选择luci-compat并且去掉勾选dnsmasq
passwall: https://github.com/xiaorouji/openwrt-passwall

安装如下两个驱动去掉勾选内置的kmod-r8169，位置kernel->network drivers
r8125最新驱动：https://github.com/goldkeyber112/openwrt-r8125
r8168最新驱动：https://github.com/BROBIRD/openwrt-r8168 不是最新

需要勾选ddns bind-host：https://github.com/sensec/ddns-scripts_aliyun 不是最新
aliyuan ddns支持：

其它推荐的内置包
luci luci下的中文语言包 opkg中文语言包
iperf3
curl
ddns
upnp
