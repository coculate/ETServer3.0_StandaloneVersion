# ETServer3.0_StandaloneVersion
照着肉饼老师的教程分离出的ET框架服务端独立版
框架作者：熊猫，社区参与者 哲学绅士，Justin沙特王子
框架地址：https://github.com/egametang/ET

肉饼老师ETServer地址：https://github.com/roubingcode/ETServer

ETServer c#游戏服务器框架
这是肉饼负责维护的一个ET框架的纯服务器版本，同步原框架更新，目前同步原框架到3.0正式版。

ET框架使用C#做服务端，现在C#是完全可以跨平台的，在linux上安装.netcore，即可，不需要修改任何代码，就能跑起来。性能方面，现在.netcore的性能非常强，比lua，python，js什么快的多了，做游戏服务端完全不在话下。

ET框架不但支持TCP，而且支持可靠的UDP协议（ENET跟KCP），ENet是英雄联盟所使用的网络库，其特点是快速，并且网络丢包的情况下性能也非常好，这个我们做过测试TCP在丢包5%的情况下，moba游戏就卡的不行了，但是使用ENet，丢包20%仍然不会感到卡，非常强大。框架还支持使用KCP协议，KCP也是可靠UDP协议，据说比ENET性能更好，使用kcp请注意，需要自己加心跳机制，否则20秒没收到包，服务端将断开连接。三种协议可以无缝切换。

ETServer运行使用方法
1.按文档 VS2017离线安装包及可能需要选择的模块 http://www.taikr.com/course/972/task/27856/show 安装好VS2017
2.下载ETServer最新版本，用VS打开项目解决方案
3.包还原后，编译解决方案中的全部项目
4.运行Server.App项目即可
