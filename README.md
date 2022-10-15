## 访问数：[![](https://visitor-badge.glitch.me/badge?page_id=sirpdboy-visitor-badge)] [![](https://img.shields.io/badge/TG群-点击加入-FFFFFF.svg)](https://t.me/joinchat/AAAAAEpRF88NfOK5vBXGBQ)
    
![screenshots](https://raw.githubusercontent.com/sirpdboy/openwrt/master/doc/说明1.jpg)

[autosamba  Auto share Samba ksmbd samba4](https://github.com/sirpdboy/autosamba)
======================
请 **认真阅读完毕** 本页面，本页面包含注意事项和如何使用。

## 功能说明：

###  自动共享 源码来源LEAN大的 autosamba自动共享脚本。

### 本着人人为我，我为人人的原则，增加自动共享Samba ksmbd samba4功能不敢独享，特分享出来，为OPENWRT添砖加瓦。


## 编译使用方法 [![](https://img.shields.io/badge/-编译使用方法-F5F5F5.svg)](#编译使用方法-)

将automount添加至 LEDE/OpenWRT 源码的方法。


### 下载源码方法：

##由于习惯问题，会和LEAN大中的autosamba冲突 ，建议编译前先删除：rm -rf package/lean/autosamba

 ```Brach
 
    # 下载源码

    git clone https://github.com/sirpdboy/autosamba package/autosamba
	
    make menuconfig
	
 ``` 
 
### 配置菜单

 ```Brach
 
    make menuconfig
	
	# 找到 LuCI -> Applications, 选择autosamba 对应的Samba ksmbd samba4, 保存后退出。
	
	# 注意：
	
	#autosamba自动共享samba，需要OPENWRT中有samba。
	
	#autosamba-ksmbd自动共享ksmbd，需要OPENWRT中有ksmbd。
	
	#autosamba-samba4自动共享samba4，需要OPENWRT中有samba4。
	
 ``` 
### 编译

 ```Brach 
 
    # 编译固件
	
    make package/autosamba/compile V=s
	
    make package/autosamba-ksmbd/compile V=s
	
    make package/autosamba-samba4/compile V=s
	
 ```

## 说明 [![](https://img.shields.io/badge/-说明-F5F5F5.svg)](#说明-)

源码来源：https://github.com/sirpdboy/autosamba

你可以随意使用其中的源码，但请注明出处。

![screenshots](https://raw.githubusercontent.com/sirpdboy/openwrt/master/doc/说明2.jpg)

# My other project

网络速度测试 ：https://github.com/sirpdboy/NetSpeedTest

定时设置插件 : https://github.com/sirpdboy/luci-app-autotimeset

关机功能插件 : https://github.com/sirpdboy/luci-app-poweroffdevice

opentopd主题 : https://github.com/sirpdboy/luci-theme-opentopd

opentoks 主题: https://github.com/sirpdboy/luci-theme-opentoks [仿KOOLSAHRE主题]

btmob 主题: https://github.com/sirpdboy/luci-theme-btmob

系统高级设置 : https://github.com/sirpdboy/luci-app-advanced

## 捐助 [![](https://img.shields.io/badge/-捐助-F5F5F5.svg)](#捐助-) 

**如果你觉得此项目对你有帮助，请捐助我们，以使项目能持续发展，更加完善。··请作者喝杯咖啡~~~**

**你们的支持就是我的动力！**

### 捐助方式

## 捐助

![screenshots](https://raw.githubusercontent.com/sirpdboy/openwrt/master/doc/说明3.jpg)

|     <img src="https://img.shields.io/badge/-支付宝-F5F5F5.svg" href="#赞助支持本项目-" height="25" alt="图飞了😂"/>  |  <img src="https://img.shields.io/badge/-微信-F5F5F5.svg" height="25" alt="图飞了😂" href="#赞助支持本项目-"/>  | 
| :-----------------: | :-------------: |
|![xm1](https://raw.githubusercontent.com/sirpdboy/openwrt/master/doc/支付宝.png) | ![xm1](https://raw.githubusercontent.com/sirpdboy/openwrt/master/doc/微信.png) |

<a href="#readme">
    <img src="https://img.shields.io/badge/-返回顶部-orange.svg" alt="图飞了😂" title="返回顶部" align="right"/>
</a>
