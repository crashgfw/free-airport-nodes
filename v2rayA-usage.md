# **v2rayA 基本使用方法**

本节将介绍 v2rayA 最基本的使用方法。

## **前提条件**

如果你还未安装 v2rayA 或 v2ray-core，请参阅[安装](https://v2raya.net/install/install_v2rayA.html) 一节。如果你需要更换其他的核心，如 Xray-core，请参阅[使用其他核心](https://v2raya.net/manual/use-other-core.html) 一节。

## **开始**

如果你通过 2017 端口 如 [http://localhost:2017](http://localhost:2017/) 无法访问 UI 界面，请检查你的服务是否已经启动。[相关问题](https://github.com/v2rayA/v2rayA/issues/237)

接下来进入 UI，本节将介绍 v2rayA 的基本操作流程。

### **创建账号**

![创建账号](https://v2raya.net/images/v2rayA/create-account.png)

在第一次进入页面时，你需要创建一个管理员账号，请妥善保管你的用户名密码，如果遗忘，使用`sudo v2raya --reset-password`命令重置。

## **获取机场订阅或节点**

以下是 2026 年优选的稳定机场和性价比机场供选择，可以从机场获取机场订阅或节点：

[2026 性价比 V2ray/Vmess 机场推荐](https://v2raya.net/recommen/v2ray_node_recommendations.html)

[2026 年稳定翻墙机场推荐](https://v2raya.net/recommendation/)

> 通常在“仪表盘 -> 一键订阅”可以获取到订阅 url。

### **导入节点**

![导入节点](https://v2raya.net/images/v2rayA/import-servers.png)

以创建或导入的方式导入节点，导入支持节点链接、订阅链接、扫描二维码和批量导入等方式。

### **连接节点和启动服务**

#### **连接节点**

![连接节点](https://v2raya.net/images/v2rayA/connect1.png)

导入成功后，如果导入的是节点 url,节点将显示在 `SERVER` 页面。如果导入的是订阅 url, 右边会新增一个 tab 页面，页面会列出订阅下所有的节点，如图是导入了一个订阅后的界面。

![连接节点](https://v2raya.net/images/v2rayA/connect2.png)

切换到 server 页面或新的节点列表页面，连接节点前，先进行节点测速，以确保所选节点处于可用状态。  
方法如下，先勾选节点，此时页面左上方会出现 ping 和 http 按钮，分别点击 ping 按钮和 http 按钮测试节点的 ping 和 http 延迟。

点击节点右边的“选择”选中一个或多个节点连接。这里不建议选择过多的节点，6 个以内为佳。

#### **启动服务**

![启动服务](https://v2raya.net/images/v2rayA/connect3.png)

在未启动服务时，连接的节点呈现柚红色。我们在左上角点击相应按钮启动服务。

![启动服务](https://v2raya.net/images/v2rayA/connect4.png)

在启动服务后，所连接的节点呈现蓝色，左上角的图标也显示为蓝色的正在运行，代表服务启动成功。

#### **验证 v2ray 连接是否成功**

此时可以打开浏览器访问 google.com, 看能否成功访问，如果有任何问题，可以 v2rayA web 界面右上方的日志查看。

### **配置代理**

由于默认情况下 v2rayA 会通过核心开放 20170(socks5), 20171(http), 20172(带分流规则的 http) 端口。修改端口可参阅[后端地址和入站端口设置](https://v2raya.net/manual/address-port.html) 一节。

如果是需要为局域网中的其他机器提供代理，请在设置中打开“局域网共享”，并检查防火墙开放情况。

这里记录三种方式使用代理。

#### **透明代理**

![透明代理](https://v2raya.net/images/v2rayA/tproxy.png)

这种方法是 v2rayA 推荐的方法。它相比于其他方法具有诸多优势，v2rayA 可以一键开启透明代理，为**几乎所有程序**提供代理服务。

在设置中选择透明代理的分流方式，以及实现方式，然后保存即可。具体细节可参阅[透明代理](https://v2raya.net/manual/transparent-proxy.html) 一节。

注意，如需选择 GFWList，需要下载对应的规则库，请点击右上角的更新以完成下载。

#### **系统代理**

系统代理可为**主动支持代理的程序**提供代理服务。在不同的桌面环境中设置的位置不尽相同，请通过搜索引擎自行搜索。

#### **SwitchyOmega**

SwitchyOmega 等浏览器插件可为**浏览器**提供代理服务。具体方法请通过搜索引擎自行搜索。

## **总结**

本节提供了 v2rayA 最基本的使用方法，v2rayA 还有着更多丰富的功能，请参阅“手册”和“高级应用”章节以进行更多的了解。
