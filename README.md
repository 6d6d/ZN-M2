<div align="center">
  <h1 align="center">
     IPQ60xx & MT798x 设备的 OpenWrt 固件发布页面
  </h1>
<a href="/LICENSE">
    <img src="https://img.shields.io/github/license/sdf8057/cloudbuild?style=flat&a=1" alt="">
  </a>
  <a href="https://github.com/sdf8057/cloudbuild/pulls">
    <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat" alt="">
  </a><a href="https://github.com/sdf8057/cloudbuild/issues/new">
    <img src="https://img.shields.io/badge/Issues-welcome-brightgreen.svg?style=flat">
  </a><a href="https://github.com/sdf8057/cloudbuild/releases">
    <img src="https://img.shields.io/github/release/sdf8057/cloudbuild.svg?style=flat">
  </a><a href="hhttps://github.com/sdf8057/cloudbuild/releases">
    <img src="https://img.shields.io/github/downloads/sdf8057/cloudbuild/total?style=flat&?">
  </a>
</div>
<br>

## ipq6000固件特性：  
0.默认后台地址192.168.1.1；默认后台密码password。  
1.添加cpu温度、频率以及npu占用率显示。  
2.修复nat环回功能失效bug。  
3.cpu超频至1.6ghz，跑分2w+。  
4.为360/和目等设备添加原厂无线校准文件。  
5.支持在线安装软件，手动安装请确保插件使用lua语言编写。  
6.释放保留内存，可用内存增加50m。  
7.此页面发布的ipq6000固件不集成无线功能。  

## 集成插件列表
luci-app-ssr-plus  
luci-app-openclash  
luci-app-ddns  
luci-app-msd_lite  
luci-app-wol  
luci-app-upnp  
luci-app-uhttpd  
luci-app-cpufreq  
luci-app-ipsec-vpnd  
luci-app-openvpn-server  
luci-app-zerotier  

luci-app-arpbind  #IP/MAC绑定
luci-app-autoreboot  #支持计划重启
luci-app-ddns   #动态域名 DNS（集成阿里DDNS客户端）
luci-app-diskman   #磁盘管理工具
luci-app-diskman ---> Include btrfs-progs   #新型的写时复制 (COW)
    luci-app-diskman ---> Include lsblk   #lsblk命令 用于列出所有可用块设备的信息
    luci-app-diskman ---> Include mdadm   #mdadm命令 用于创建、管理、监控RAID设备的工具
    luci-app-diskman ---> Include kmod-md-raid456   #RAID 4,5,6 驱动程序模块（丢弃）
    luci-app-diskman ---> Include kmod-md-linear   #RAID 驱动程序模块（丢弃）
luci-app-docker  #Docker容器
luci-app-dockerman  #Dockerman容器  *
luci-app-filetransfer  #文件传输（可web安装ipk包）
luci-app-netdata  #Netdata实时监控（图形化）
luci-app-nlbwmon   #网络带宽监视器
luci-app-openclash  #运行在OpenWrt上的Clash代理客户端（Le库以外的插件）
luci-app-samba   #网络共享（Samba）
luci-app-samba4   #网络共享（Samba4）
luci-app-serverchan   #微信/请不要发布这类群，谢谢推送的插件
luci-app-socat  #Socat多功能的网络工具(端口转发)   *
luci-app-sqm  #流量智能队列管理（QOS）
luci-app-ttyd   #网页终端命令行
luci-app-turboacc   #Turbo ACC 网络加速(支持 Fast Path 或者 硬件 NAT)
    luci-app-turboacc ---> Include Flow Offload   #Flow Offload加速(提高路由转发效率)  *
    luci-app-turboacc ---> Include Shortcut-FE  #Shortcut-FE 流量分载
    luci-app-turboacc ---> Include Shortcut-FE CM   #Shortcut-FE 流量分载(高通芯片版)  *
    luci-app-turboacc ---> Include BBR CCA  #BBR拥塞控制算法提升TCP网络性能
    luci-app-turboacc ---> Include Pdnsd   #DNS防污染 Pdnsd  *
    luci-app-turboacc ---> Include DNSForwarder  #DNS防污染 Forwarder
    luci-app-turboacc ---> Include DNSProxy  #DNS防污染 Proxy
luci-app-uhttpd  #uHTTPd Web服务器
luci-app-upnp   #通用即插即用UPnP（端口自动转发）
luci-app-verysync  #微力同步
luci-app-vsftpd  #FTP服务器
luci-app-watchcat  #断网检测功能与定时重启
luci-app-wol   #WOL网络唤醒
luci-app-wrtbwmon  #实时流量监测
luci-app-mjpg-streamer   #兼容Linux-UVC的摄像头程序

## 固件预览
![image](https://github.com/sdf8057/cloudbuild/blob/main/pic/overview.png)

## 微信打赏
![image](https://github.com/sdf8057/cloudbuild/blob/main/pic/reward_qrcode.png)
