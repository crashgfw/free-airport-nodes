# 2025 最新科学上网方式汇总

在本文中，我们将探讨多种科学上网的方法，通过分析不同技术手段的特点，帮助你根据个人的实际应用需求和现有设备，选择合适的翻墙方式。此外，针对一些常见的科学上网问题，我们也会提供简明扼要的解答。

## 1. 软件翻墙

### 1.1. VPN 虚拟私有网络

虚拟私有网络（VPN）曾经是非常流行的翻墙工具之一。最初是为金融交易或是公司、团体保密通信等内部通信提供安全性而设计的技术，在 GFW 早期阶段，人们开始将 VPN 应用于绕开网络审查。VPN 通过加密和隧道化技术，将你的数据流量从你的设备发送到 VPN 服务器，然后再由服务器发送到目标网站，从而实现突破 GFW 的封锁。

然而，现代 VPN 的流量特征已经被 GFW 完全识别，使其不再是可靠的翻墙方式，经常在某些敏感时期进行集体休假。

此外，国内一些不安全的套壳伪 VPN 服务极有可能导致个人信息泄露，因此强烈建议谨慎选择（如某连、某王、某鲸等，及一众免费钓鱼 VPN）。

-   优点：提供端对端加密，保护通信隐私；也可以访问某些被封锁的网站；
-   缺点：现代 VPN 流量特征被 GFW 识别，不再是可靠的翻墙方式；不安全的 VPN 极有可能导致信息泄露。

### 1.2. 代理上网

基于代理协议的翻墙软件是近几年逐渐兴起的新的翻墙手段，目前被绝大多数科学上网用户选择的主流方式。机场代理服务商通常提供使用 Shadowsocks、Shadowsocks R、VMess、 Vless、Trojan 等加密协议编写的节点服务器，用户只需要将节点订阅文件粘贴导入各种开源的翻墙软件中，即可实现本地与远程服务器间应用层流量代理突破封锁。

由于这些新兴的代理协议的目的就是绕过 GFW 的封锁，所以针对性地做了优化，实现更适合大数据高速传输的效果。这使得在访问被限制的网站时，机场相比 VPN 在数据传输速度和稳定性方面表现更出色。

机场发展初期运行节点代理协议的开源软件主要是 Shadowsocks、Shadowsocks R（这里指开源应用软件，与上文协议文件同名），目前 Shadowsocks、ShadowsocksR 也逐渐被 GFW 识别拦截，VMess、VLess、Trojan、Hysteria 等代理协议逐渐取代 SS 和 SSR 作为直连节点的代理协议， SS 和 SSR 由于其性能方面的优势，仍然作为中转落地节点的主要协议。

| 机场客户端                                                 | 支持的协议                                                 | 官网                                 |
| :--------------------------------------------------------- | :--------------------------------------------------------- | ------------------------------------ |
| Clash(Windows, MacOS, Android, OpenWRT)                    | SS/SSR/VMess/Trojan                                        |                                      |
| Clash meta(Windows, Linux, macOS, Android, iOS)            | SS/SSR/VMess/Trojan/Hysteria 2/Tuic                        |                                      |
| Stash( MacOS & IOS)                                        | SS/SSR/VMess/Trojan/Hysteria 2                             |                                      |
| Shadowrocket(IOS)                                          | SS/SSR/VMess/Trojan/Hysteria 2/Tuic                        |                                      |
| Surge(MacOS & IOS)                                         | SS/SSR/VMess/Trojan/Hysteria 2                             |                                      |
| V2rayA(Windows, Linux, MacOS, OpenWRT)                     | SS/SSR/VMess/Trojan/Juicity/Tuic                           | [官网](https://v2raya.org/)          |
| V2rayN(Windows)                                            | SS/SSR/VMess/Trojan/Hysteria2                              |                                      |
| V2rayNG(Android)                                           | SS/SSR/VMess/Trojan                                        |                                      |
| Surfboard(Android)                                         | SS/SSR/VMess/Trojan                                        |                                      |
| Sing-box(Windows, MacOS, Android, IOS, Apple TV)           | SS/SSR/VMess/Trojan/Hysteria 2                             |                                      |
| Hiddify Next(Windows, MacOS, Linux, Android, IOS, OpenWrt) | SS/SSR/VMess/Trojan/Hysteria 2                             | [官网](https://hiddify.com)          |
| Furious(Windows, MacOS, Linux)                             | SS/SSR/VMess/Trojan/Hysteria 2                             |                                      |
| Clash Nyanpasu(Windows, MacOS, Linux)                      | SS/SSR/VMess/Trojan/Hysteria 2/WireGuard                   | [官网](https://nyanpasu.elaina.moe/) |
| PassWall2(OpenWRT)                                         | SS/SSR/VMess/Trojan/Hysteria 2/Socks5/TUIC/WireGuard/Vless |                                      |
| Quantumult X (IOS)                                         | SS/SSR/VMess/Trojan                                        |                                      |
| ShadowSocksR Plus+(OpenWRT)                                | SS/SSR/VMess/Trojan/WireGuard/VLess                        |                                      |

> Clash meta A rule-based tunnel in Go (v1.16.0 后支持 Hysteria 2)
> Shadowrocket Rule based proxy utility client for iPhone/iPad (2.2.35 后支持 Hysteria 2)
> Stash Simple & Powerful Network Tool (2.5.0 后支持 Hysteria 2)
> Surge Advanced Network Toolbox (5.8.0 后支持 Hysteria 2)
> V2rayN 需要将内核替换 Hysteria2 以支持 Hysteria 2

更多代理上网软件列举如下： [Furious](https://github.com/LorenEteval/Furious)，[NekoRay](https://github.com/Matsuridayo/nekoray), [HiddifyN](https://github.com/hiddify/HiddifyN), [X-flutter](https://github.com/XTLS/X-flutter), [Mango](https://github.com/arror/Mango), [foxray](https://apps.apple.com/app/foxray/id6448898396), [Streisand](https://apps.apple.com/app/streisand/id6450534064), [V2rayU](https://github.com/yanue/V2rayU), [Passwall2](https://github.com/xiaorouji/openwrt-passwall2), [openwrt-xray](https://github.com/yichya/openwrt-xray), [V2RayW](https://github.com/Cenmrev/V2RayW)，[Clash Verge](https://github.com/zzzgydi/clash-verge/tree/main)，
[V2RayX](https://github.com/Cenmrev/V2RayX)，[Qv2ray](https://github.com/Qv2ray/Qv2ray), [wireproxy](https://github.com/pufferffish/wireproxy)，[naiveproxy](https://github.com/klzgrad/naiveproxy)。

-   优点： 使用不同的协议和加密方式，确保数据的安全性；更换不同机场只需更换订阅链接即可，不用重新下载客户端；

## 2. 硬件翻墙

### 2.1. 路由器翻墙

有时候，软件翻墙可能会受到设备特性的限制无法实现。因此，考虑使用硬件翻墙的方式更为合适。路由器翻墙是将翻墙软件部署在路由器上，从而实现对整个局域网的翻墙。这样，无论是 TV、电脑、手机、平板、家用游戏主机、VR 头显还是其他设备，只要连接到同一个路由器，都可以实现翻墙访问。

然而，路由器翻墙也存在性能瓶颈，需要注意路由器的 CPU 处理能力是否足够满足多设备的翻墙需求。

-   **优点：** 方便，无需在每个设备上安装翻墙软件；
-   **缺点：** 路由器的 CPU 性能可能限制网络速度，需要选择性能足够的路由器。

### 2.2. 软路由翻墙

软路由是一种改造过的路由器，性能较强，能够实现更复杂的网络功能。使用软路由可以更好地满足多设备翻墙需求，但同时也需要较高的技术门槛，涉及到虚拟机 Linux 这些相关的知识，配置相对复杂，且价格较高。

另外相比其他方式，软路由维护也挺麻烦，就是固件更新节点切换都要进入后台操作。因此，是否需要软路由取决于你的技术水平和需求。

-   **优点：** 性能出色，完全不用考虑各种设备运算能力导致的网络传输延迟问题；
-   **缺点：** 成本可能较高，配置相对复杂，需要更多的技术知识。

### 2.3. 网关翻墙

通过在本地局域网里面部署运行 **Clash For Windows** 或 **Surge For Mac** 的电脑当做网关，接管局域网里面其他网络设备的所有流量实现全局透明代理。

相比较其他的硬件代理模式，不仅计算机运算能力强大，而且操作上也异常的便捷，有的软件甚至只需要点击局域网模式即可实现，完全不用单独再采购昂贵的软路由设备。

-   **优点：** 全局代理包括应用层、系统层和硬件层的通信，操作简便。
-   **缺点：** 需要一台计算机长时间开机以保持翻墙状态。

## 3. 翻墙协议介绍

### 3.1. VPN

VPN（Virtual Private Network，虚拟私人网络）是一种常用于连接中、大型企业或团体与团体间的私人网络的通讯方法。虚拟私人网络的讯息透过公用的网络架构（例如：互联网）来传送内联网的网络讯息。它利用已加密的通道协议（Tunneling Protocol）来达到保密、发送端认证、消息准确性等私人消息安全效果。

正常网络通信时，所有网络请求都是通过我们的物理网卡直接发送出去。而 VPN 是客户端使用相应的 VPN 协议先与 VPN 服务器进行通信，成功连接后就在操作系统内建立一个虚拟网卡，一般来说默认 PC 上所有网络通信都从这虚拟网卡上进出，经过 VPN 服务器中转之后再到达目的地。

通常 VPN 协议都会对数据流进行强加密处理，从而使得第三方无法知道数据内容，这样就实现了翻墙。翻墙时 VPN 服务器知道你干的所有事情（HTTP，对于 HTTPS，它知道你去了哪）。

VPN 具有多种协议，常见的有以下几种：

1.  PPTP（Point-to-Point Tunneling Protocol，点对点隧道协议）：是最早的 VPN 协议之一，使用较广泛，具有快速、易于设置等优点，但安全性不如其他协议。
2.  L2TP（Layer Two Tunneling Protocol，第二层隧道协议）：在 PPTP 的基础上进行改进，加入了 IPSec 协议，提高了安全性和稳定性，但速度相对较慢。
3.  IPSec（Internet Protocol Security，互联网协议安全）：是一种较为安全的 VPN 协议，支持多种加密算法和认证方式，能够提供强大的安全保障，但配置较为复杂。
4.  SSL/TLS（Secure Sockets Layer/Transport Layer Security，安全套接字层/传输层安全）：是一种基于加密的 VPN 协议，不需要额外的客户端软件，具有易用性和安全性高等特点，但相对较慢。

**特征检测**

要想成功翻墙都必须与对应的远程服务器建立连接，然后再用对应的协议进行数据处理并传输。
而问题就出在这里：翻墙工具和远程服务器建立连接时，如果表现的很独特，在一大堆流量里很显眼，就会轻易被 GFW 识别出从而直接阻断连接，而 VPN（尤其是 OPENVPN）和 SSH 这方面的问题尤其严重。

### 3.2. Shadowsocks

Shadowsocks 是一种基于 SOCKS5 代理的加密传输协议，主要用于科学上网和绕过网络审查。它由开发者 clowwindy 于 2012 年创建，旨在提供一种简单、高效且难以被检测的代理工具。

Shadowsocks 通过在客户端和服务器之间建立加密隧道来传输数据。客户端将流量加密后发送到 Shadowsocks 服务器，服务器解密后再将请求转发到目标网站。返回的数据同样经过加密传输回客户端。使用对称加密算法（如 AES、ChaCha20、Salsa20 等）对数据进行加密，确保传输的安全性。协议设计简单，资源占用低，适合在低性能设备（如路由器）上运行。

### 3.3. V2Ray/Vmess 协议

最后来说说近年很红的 V2Ray. 技术细节可以参考 V2Ray Beginniner's Guide。或是 GitHub <https://github.com/v2fly/v2ray-step-by-step>

V2Ray 的运行原理与其他代理工具基本相同，使用特定的中转服务器完成数据传输。例如，用户无法直接访问 Google，YouTube 等网站，但代理服务器可以访问，且用户可以直接连接代理服务器，那么用户就可以通过特定软件连接代理服务器，然后由代理服务器获取网站内容并回传给用户，从而实现代理上网的效果。服务器和客户端软件会根据不同协议，要求用户提供一定的参数，如 UUID、密钥、加密方式等，双方一致后才能成功连接（VMess 协议能够自适应客户端采用的加密方式）。连接到服务器后，客户端会在本机构建一个本地 Socks5 代理（或 VPN、HTTP、透明代理等）。浏览网络时，客户端通过这个 Socks5（或其他形式）代理收集网络流量，然后再经混淆加密发送到服务器端，以防网络流量被识别和拦截，反之亦然。

V2Ray 定位为一个平台，任何开发者都可以利用 V2Ray 提供的模块开发出新的代理软件。具有各种分层代理协议、传输和混淆。例如，您可以在一个端口上运行 SOCKS-in-TLS，在另一个端口上运行 VMess-in-QUIC（可以选择混淆 QUIC 数据包）。在客户端，您可以配置路由来控制什么流量应该使用什么代理，或者根本不应该被代理。

VMess 是一个加密传输协议，它分为入站和出站两部分，通常作为 V2Ray 客户端和服务器之间的桥梁。

VMess 依赖于系统时间，请确保使用 V2Ray 的系统 UTC 时间误差在 90 秒之内，时区无关。在 Linux 系统中可以安装 ntp 服务来自动同步系统时间。

### 3.4. Vless 协议

VLESS 是一个无状态的轻量传输协议，它分为入站和出站两部分，可以作为 V2Ray 客户端和服务器之间的桥梁。

与 VMess 不同，VLESS 不依赖于系统时间，认证方式同样为 UUID，但不需要 alterId。

### 3.5. Trojan 协议

Trojan 协议是一种基于 TLS 加密的代理协议，主要用于绕过网络审查和防火墙。它通过伪装成正常的 HTTPS 流量来隐藏代理通信，使其难以被检测和封锁。Trojan 协议的核心特点包括：

-   TLS 加密：所有通信都通过 TLS 加密，确保数据安全性和隐私。
-   伪装流量：Trojan 流量与正常的 HTTPS 流量几乎无法区分，增加了隐蔽性。
-   轻量高效：协议设计简洁，性能开销低，适合在低带宽或高延迟的网络环境中使用。
-   抗检测：通过混淆技术，Trojan 能够有效规避深度包检测（DPI）等审查手段。

Trojan 协议通常与 Web 服务器（如 Nginx）结合使用，进一步隐藏代理流量，使其看起来像正常的 Web 访问。由于其高效性和隐蔽性，Trojan 在需要绕过网络限制的场景中广受欢迎。

### 3.6. TUIC v5 协议

TUIC V5，TUIC 是一种网络代理协议，专注于尽可能减少中继导致的额外握手延迟，并保持协议本身的简单易实现，TUIC 最初设计用于 QUIC 协议之上，但理论上可以将其与任何其他协议一起使用，比如 TCP 协议，它可以充分利用 QUIC 带来的优势。

### 3.7. Juicity 协议

Juicity 协议是一个开源的网络代理协议，作者在开发 Juicity 协议时受到了 TUIC 的启发。Juicity、TUIC、Hysteria 协议一样，均基于 QUIC（Quick UDP Internet Connections）协议实现。QUIC 是一个由 Google 开发的基于 UDP 的传输层网络协议，旨在减少连接和传输延迟。Juicity 与 Hysteria 不同之处主要为使用的拥塞算法，Juicity 可以使用的拥塞算法包括 reno、cubic、bbr 和 bbr2 ，而 hysteria 可以使用 brutal 拥塞算法。 brutal 拥塞算法表现的更为霸道与暴力，因此在网络链路不好的情况下，Hysteria 协议比 Juicity 协议的传输速度要快一些。

### 3.8. Hysteria 2

Hysteria 2 是一个开源的网络加速工具，它是 Hysteria 的第二个版本。Hysteria 是一个基于 UDP 的网络加速工具，旨在提高网络连接的速度和稳定性。Hysteria 2 在原有的基础上进行了一些改进和优化，以提供更好的性能和用户体验。

Hysteria 2 的主要特点包括：

-   高性能：通过使用更高效的算法和技术，Hysteria 2 能够提供更快的网络速度和更稳定的连接。
-   易用性：Hysteria 2 提供了简单易用的命令行界面和配置选项，使得用户可以轻松地设置和使用。
-   跨平台支持：Hysteria 2 支持多种操作系统，包括 Windows、macOS、Linux 等，使得用户可以在不同的平台上使用。
-   开源：Hysteria 2 是开源的，这意味着用户可以查看其源代码，并根据需要进行修改和定制。

Hysteria 2 的开发目标是为用户提供一个高效、稳定、易用的网络加速工具，以满足不同的网络需求。

### 3.9. NaiveProxy

NaiveProxy，挪威语叫 NaïveProxy，翻译成中文：“天真的代理”，是 2019 年底由 klzgrad 大神开发的一种突破 GFW 网络审查的新型科学上网代理技术，它使用 Chrome 的网络堆栈来伪装流量，具有较强的抗审查能力和较低的可检测性，重用 Chrome 网络堆栈是确保性能和安全性的最佳实践。

NaiveProxy 的原理和 trojan 很像，除去教程搭建的节点消除了服务器 tls 指纹和隐藏了所有翻墙服务以及伪装成正常网站，NaiveProxy 协议更上一层，消除了客户端的 tls 指纹和 tls-in-tls 特征，并且 naive 协议基于 http2，自带多路复用，对比 ws 需要频繁握手来讲延迟更低，前面也说过 NaiveProxy 客户端使用 chrome 浏览器内核作为网络协议栈，从防火墙的角度来看，就像是你在正常的使用正常的谷歌浏览器访问正常的网站。