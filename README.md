# 免责声明🧐
本工具仅面向 **合法授权** 的企业安全建设行为，如您需要测试本工具的可用性，请自行搭建靶机环境。

在使用本工具进行检测时，您应确保该行为符合当地的法律法规，并且已经取得了足够的授权。**请勿对非授权目标进行扫描**。

如您在使用本工具的过程中存在任何非法行为，您需自行承担相应后果，我们将不承担任何法律及连带责任。

在安装并使用本工具前，**请您务必审慎阅读**、充分理解各条款内容，限制、免责条款或者其他涉及您重大权益的条款可能会以加粗、加下划线等形式提示您重点注意。 除非您已充分阅读、完全理解并接受本协议所有条款，否则，请您不要安装并使用本工具。您的使用行为或者您以其他任何明示或者默示方式表示接受本协议的，即视为您已阅读并同意本协议的约束。

# 工具来源
```
（1）nps通信流量比较稳定，但特征抓的比较死，所以基于原版的nps进行二次开发
```
# 魔改部分

```
（1）重写了nps的认证过程，通信过程均进行加密
（2）重些了npc的部分，预计后续分离config文件进行加载
（3）进行了nps未授权漏洞的修复，避免了默认配置未授权
```



# 免杀情况
（这是魔改后的demo上去的，还请各位测试切莫进行☁️测试、沙箱测试、联网测试）
### virustotal
<img width="1244" alt="image" src="https://github.com/Q16G/npsmodify/assets/113832601/24f0dc87-e3d9-4ef0-b2fb-c9316b3a473f">

### windows defender（静态）
<img width="1154" alt="image" src="https://github.com/Q16G/npsmodify/assets/113832601/bdd32ed9-cf3d-46e5-b53b-c37d890e8a80">

### windows defender（动态）
<img width="1492" alt="image" src="https://github.com/Q16G/npsmodify/assets/113832601/50cbabc4-641d-48cd-8828-fbbd21dc1c3e">


### 360、火绒等其他杀软未进行测试


# 项目使用
未进行测试nps服务端的注册，所以目前主要还是 ./nps的方式来运行
## 服务端使用
<img width="802" alt="image" src="https://github.com/Q16G/npsmodify/assets/113832601/79db09cb-72f7-454b-a2e8-aee2aa25ef5f">


## 客户端使用

### 配置文件启动
<img width="768" alt="image" src="https://github.com/Q16G/npsmodify/assets/113832601/efe78eb9-7a45-44ef-aa3c-5d59b7498e50">

### 命令行启动
<img width="787" alt="image" src="https://github.com/Q16G/npsmodify/assets/113832601/d62ab71c-1fee-48a9-85e7-35180f0a83e0">



# 项目进度

✅ 2023.5.19 重新写了通信认证协议

✅ 2023.5.20 把连接流量进行混淆，仅仅支持客户端命令行启动，未支持conf文件启动

✅ 2023.5.21 支持本地config文件加载

# 后续增加
   （1）~~增加config文件分离，实现远端拉取~~（估计很快）
   
   （2）~~实现其他流量的魔改~~
# 参考
```
https://github.com/ehang-io/nps
```

