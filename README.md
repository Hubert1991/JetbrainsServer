# JetBrains Server

`version 0.1.1`
`20180504`

It is a Shell Script which can build a JetBrains Server automatically.

---

`HOW TO USE`

```sh
wget --no-check-certificate -O install.sh https://raw.githubusercontent.com/Hubert1991/JetbrainsServer/master/install.sh && chmod +x install.sh && bash install.sh
```

> **License server http://ip:1026**



##### firewall

```sh
iptables -I INPUT -m state --state NEW -m tcp -p tcp —dport 1026 -j ACCEPT
iptables -I INPUT -m state --state NEW -m udp -p udp —dport 1026 -j ACCEPT

firewall-cmd --zone=public --add-port=1026/tcp
firewall-cmd --zone=public --add-port=1026/udp
firewall-cmd --zone=public --add-port=1026/tcp --permanent
firewall-cmd --zone=public --add-port=1026/udp --permanent
```

---

The following hardware platforms and operating systems are supported. More  hardware platforms and operating systems are coming.

| Hardware Platform | Operating System            |
| ----------------- | --------------------------- |
| x86/i386          | Debian、Ubuntu、CentOS        |
| x86-64/amd64      | Debian、Ubuntu、CentOS、Deepin |
| Raspberry pi      | Raspbian                    |

This following JetBrains products are supported:

- AppCode
- CLion
- DataGrip
- dotCover
- dotMemory
- dotTrace
- IntelliJ IDEA
- GoLand
- PhpStorm ( 最新支持到 2018.2 )
- PyCharm
- ReSharper
- ReSharper C++
- ReSharper Ultimate
- Rider
- RubyMine
- WebStorm



(Binaries from blog.lanyus.com)
