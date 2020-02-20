# luci-app-vssr
a new SSR SS V2ray luci app bese luci-app-ssr-plus

#### Intro
写在前面：插件改名的原因并非是要另起炉灶，主要是自己想要的功能【视觉体验优先】，和原版略有差异，而且插件体积越来越大，并不适合小ROM机器使用。

1.基于lean ssr+ 全新修改的Vssr（更名为Hello World） 主要做了很多的修改和优化，同时感谢插件原作者所做出的的努力和贡献！

2.节点列表支持国旗显示 TW节点为五星红旗， 节点列表页面 打开自动ping.

3.优化了在节点列表页面点击应用后节点切换的速度。同时也优化了自动切换的速度。

4.给Hello World 增加了IP状态显示，在页面底部 左边显示当前节点国旗 ip 和中文国家 右边 是四个网站的访问状态  可以访问是彩色 不能访问是灰色。

5.优化了国旗匹配方法，在部分带有emoji counrty code的节点名称中 优先使用 emoji code 匹配国旗。

6.建议搭配opentomato  opentomcat  theme，能有最好的显示体验。

新修改插件难免有bug 请不要大惊小怪。欢迎提交bug。

###  此版本已和魔改版合并

#### Notice
需要的依赖有python3-maxminddb libmaxminddb 请自行添加

#### 感谢
https://github.com/coolsnowwolf/lede

#### My other project
Argon theme ：https://github.com/jerrykuku/luci-theme-argon
      
theme : https://github.com/Leo-Jo-My/luci-theme-opentomato

theme : https://github.com/Leo-Jo-My/luci-theme-opentomcat

theme : https://github.com/Leo-Jo-My/luci-theme-Butterfly

openwrt-nanopi-r1s-h5 ： https://github.com/jerrykuku/openwrt-nanopi-r1s-h5

### 说明

源码来源：https://github.com/jerrykuku/luci-app-vssr

### 使用方法
```Brach
    #下载源码
    
    git clone https://github.com/Leo-Jo-My/luci-app-vssr package/luci-app-vssr
    
    git clone https://github.com/Leo-Jo-My/my package/my  #依赖包
    
    make menuconfig
    
    #编译
    
    make package/luci-app-vssr/{clean,compile} V=s


