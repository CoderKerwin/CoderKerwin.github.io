# APPLICATION SOFTWARE

## EDITOR

### VIM

<https://www.vim.org>, <https://github.com/vim>, <https://github.com/neovim/neovim>

<https://github.com/termux/termux-app>, <https://f-droid.org/en/packages/com.termux>

<https://github.com/jackpal/Android-Terminal-Emulator>

<https://github.com/shiftrot/droidvim>

<https://github.com/rhysd/vim.wasm>,
<https://neovim.discourse.group/t/run-neovim-in-browser-via-wasm/3997>,
<https://neovim.discourse.group/t/compile-to-webassembly/2736>,
<https://nvim.nry.app>

不能通过`@*`方式向ssh的vim传递剪切板，只能通过右键或Ctrl_V方式传递，相当于一个个字符输入

### VSCODE

[Bundling Extensions](https://code.visualstudio.com/api/working-with-extensions/bundling-extension)

[VSCE command](https://michaelcurrin.github.io/dev-cheatsheets/cheatsheets/other/vscode-extensions/vsce-command.html): `vsce package` to generate vsix file

[Find and fix problems in your JavaScript code](https://eslint.org): <https://github.com/microsoft/vscode-eslint>

[发行VSCODE插件](https://zhuanlan.zhihu.com/p/339695661)

```shell
npm i vsce ts-loader eslint
./node_modules/.bin/vsce package
```

```shell
curl -L -O https://github.com/neovim/neovim/releases/download/v0.9.5/nvim-linux64.tar.gz
tar xzvf nvim-linux64.tar.gz
find nvim-linux64 -name nvim
```

## CODEVIEWER

### OPENGROK
[OPENGROK](https://opengrok.github.io)

### CODE-SERVER
[CODE-SERVER](https://github.com/coder/code-server):
<https://github.com/coder/coder/releases>

### CSCOPE
[CSCOPE](https://github.com/yifengyou/cscope),
[CSCOPE](https://github.com/Hyeonykim/cscope),
[CSCOPE](https://github.com/youyuanwu/cscope),
[CSCOPE](https://github.com/Smattr/clink)

## COMPILER

### C/C++ COMPILER

#### MSVC

[MSVC编译器参考](https://learn.microsoft.com/zh-cn/cpp/build/reference/compiling-a-c-cpp-program?view=msvc-170)

#### GCC

[GNU Compiler Collection          ](https://gcc.gnu.org),
[Options That Control Optimization](https://gcc.gnu.org/onlinedocs/gcc/Optimize-Options.html)

[GCC基本使用](https://zhuanlan.zhihu.com/p/404682058)

#### CLANG

#### KEIL

[stc-isp安装教程win11_stcisp安装教程win11](https://www.keil345.com/keil/108528.html)

[STC-ISP单片机烧录软件](http://www.i5wz.com/soft/bckf/11509.html)

## JAVA COMPILER

Bing: OpenJDK download,
<https://jdk.java.net/archive>,
<https://download.java.net/java/GA/jdk11/9/GPL/openjdk-11.0.2_windows-x64_bin.zip>

### OPENJDK

## ANALYSIS

### COVERITY

### KLOCKWORK

## UNITTEST

[OpenCppCoverage](https://github.com/OpenCppCoverage/OpenCppCoverage),
[C++开源代码覆盖率工具OpenCppCoverage介绍(Windows)](https://www.cnblogs.com/coderzh/p/OpenCppCoverage.html),
[GCOV使用    ](https://blog.csdn.net/lishenglong666/article/details/8056777),
[gcov使用小节](https://blog.csdn.net/weixin_41910194/article/details/80759473)

### CMOCKA

## DISASSEMBER
readelf, nm, objdump, dumpbin

### DUMPBIN

### OBJDUMP

### NM

### IDA

## DEBUGGER

### GDB
[Options for Debugging Your Program](https://gcc.gnu.org/onlinedocs/gcc/Debugging-Options.html)

[gdb调试用法](https://www.cnblogs.com/ims-/p/10529393.html),
[GDB调试教程](https://geekdaxue.co/read/myheros@pkwqzc/pqq09f)

编译选项：-g

gdb命令`b/bt/c/d/h/i/n/p/q/r/s/x/mem/display`，详细如下  
b  : break at  
bt : stack trace  
c  : continue  
d  : delete breakpoints  
h  : help  
i  : info, belong status query  
i b: info breaks  
i r: info registers  
n  : next  
p  : print /FMT  
q  : quit  
r  : run  
s  : step  
x  : examine /FMT is /x /c /d /b etc

symbol-file : load symbol. ``symbol-file -o `offset` `FILE` ``

mem         : show memory  
display     : display variable  
disassemble : disassemble. /r /s modifier  
list        : list source of function or line

[GDB用法详解](https://www.cnblogs.com/lvdongjie/p/8994092.html)

### WINDBG

编译选项：Zi, /debug

windbg命令`bp/d/g/gc/k/p/q/r/t/x`，详细如下
bp  : break  
d   : display memory.  
dt  : display type  
dv  : display local variable  
dx  : display C++ expression. `dx -r1 (*((Test!_EFI_PLATFORM_INFO *)0x0))`  
g   : go  
gc  : go in condition  
k   : stack frame  
lm  : load module. !lmi can show information as well  
p   : single instruction  
q   : quit  
r   : register  
t   : trace  
u   : unassemble  
ub  : unassemble  
uu  : unassemble  
uf  : unassemble function  
x   : examine symbol. /D /t /v  
.hh : help

[Debugging Tools for Windows (WinDbg, KD, CDB, NTSD)](https://learn.microsoft.com/en-us/windows-hardware/drivers/debugger)
[Debug Help Library                                 ](https://learn.microsoft.com/en-us/windows/win32/debug/debug-help-library)
[SymGetTypeInfo function                            ](https://learn.microsoft.com/en-us/windows/win32/api/dbghelp/nf-dbghelp-symgettypeinfo)
[PE Format                                          ](https://learn.microsoft.com/en-us/windows/win32/debug/pe-format)

[linux/windows下查看目标文件.a/.lib的函数符号名称](https://blog.csdn.net/listener51/article/details/77266824)

### DBH

dbh.exe可以直接看symbol
t      : type symbol
x      : enum symbol
q      : quit
r      : show source file
etypes : show all type

## ASSEMBLER

### NASM

## BUILDER
软件构建：ant/nant/gradle/cmake/make/nmake/msbuild

### MAKE

### NMAKE

### MSBUILD

### ANT

### GRADLE

### CMAKE

### EDK2-BASETOOLS

## DOCUMENTATION

### DOXYGEN

<http://www.doxygen.nl/download.html>

### [PLANTUML](https://plantuml.com)

### [MERMAID](https://mermaid.js.org)

### READTHEDOC

https://about.readthedocs.com

### SPHINX

https://www.sphinx-doc.org

[Clear, Functional C++ Documentation with Sphinx + Breathe + Doxygen + CMake](https://devblogs.microsoft.com/cppblog/clear-functional-c-documentation-with-sphinx-breathe-doxygen-cmake)

[Sphinx + Read the Docs 从懵逼到入门](https://zhuanlan.zhihu.com/p/264647009)

### GITBOOK

### GITHUB.IO

Tianocore项目使用了github.io来做为文档展示，参考这个来构建github.io网页：
[github.io](https://pages.github.com),
[Quickstart for GitHub Pages](https://docs.github.com/en/pages/quickstart),
[Approving a pull request with required reviews](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/approving-a-pull-request-with-required-reviews),
[Pulls](https://docs.github.com/en/rest/pulls/pulls?apiVersion=2022-11-28)

### CONFLUENCE
[CONFLUENCE](https://www.atlassian.com/software/confluence)

### MEDIAWIKI
[MEDIAWIKI](https://www.mediawiki.org)

### SPHINX
[Sphinx](https://www.sphinx-doc.org): Python Documentation Generator

[Sphinx theme](https://github.com/readthedocs/sphinx_rtd_theme)

### COMPARE

| GITBOOK                                             | GITHUB                                                |
|-----------------------------------------------------|-------------------------------------------------------|
| Provide space to save document but not provide tool | Provide space to save document but not provide tool   |
| Can link to GITHUB or other source control website  | Only support GITHUB website                           |
| Support search                                      | Not support search but can goto repository for search |

| SPHINX      | DOXYGEN  | PLANTUML      |
|-------------|----------|---------------|
| Python      | C        | Java          |
| More Plugin | N/A      | It's plugin   |
| For Docs    | For Docs | For Diagrams  |

## CI
持续开发(CI/CD)

[TeamCity](https://www.jetbrains.com/teamcity),
[TeamCity VS Jenkins：选择正确的CI / CD工具](https://cloud.tencent.com/developer/article/1664894),
[谁才是世界上最好的 CI/CD 工具？](https://zhuanlan.zhihu.com/p/67805669),
[Azure DevOps](https://azure.microsoft.com/en-us/products/devops)

## NETWORK
`systemctl status networking`, `/etc/systemd/system/network*`, `/lib/systemd/system/network*`, `/sbin/ifup`, `/etc/network/if-up.d`, `/etc/network/interfaces`

`/lib/systemd/system/networking.service`会调用`ifup`，`ifup`会调用`/etc/network/if-up.d/wpasupplicant`，但因为`/etc/network/interfaces`里面没有wpa相关配置，所以wpasupplicant只跑了`start()`就退出了。  
`networking.service`在`wpa_supplicant.service`之前运行，所以networking由于wpa为准备好无法正常配置dhcp。  
当前暂时改了`/etc/network/interfaces`与`wpasupplicant`两个文件解决debian无法配置开机自动配置wifi问题。

`/sbin/init`是指向`/sbin/systemd`的软链接

### IPTABLES
<https://packages.debian.org/buster/iptables>,
<https://www.netfilter.org>,
<https://www.frozentux.net/iptables-tutorial/iptables-tutorial.html>

[Windows配置双网卡多网卡路由表](https://www.cnblogs.com/Chary/p/13957475.html)

### VPS
<https://www.vpstop.cn>

### FRP
[frp内网穿透](https://itlanyan.com/frp-tunnel-tutorial),
<https://github.com/fatedier/frp/releases>,

### PROXY
[Linux配置成代理服务器](https://www.cnblogs.com/caopeng/p/17909476.html),
<https://www.digitalocean.com/community/tutorials/how-to-set-up-squid-proxy-for-private-connections-on-debian-11>,

### OPENVPN
<https://ubuntu.com/server/docs/how-to-install-and-use-openvpn>,
<https://documentation.ubuntu.com/server/how-to/security/install-openvpn>,
<https://github.com/openvpn>,
<https://openvpn.net/community>,
<https://www.doncaprio.com/how-to-create-a-personal-vpn-openvpn-on-your-vps>,
[OpenVPN配置代理路由实现局部代理](https://www.luisimon.com/2020/04/25/318),
[手把手教你搭建OpenVPN](https://blog.admin4j.com/linux/vpn),
[openvpn配置实现服务器代理上网](https://blog.csdn.net/java_linux_dev/article/details/135879838),
[搭建OpenVpn实现服务器代理上网](https://blog.csdn.net/weixin_44105868/article/details/139463173),
<https://blog.desdelinux.net/zh-CN/如何创建您的VPN服务器>,
[Debian10搭建openvpn](https://blog.csdn.net/m0_57832432/article/details/124412513),
<https://www.debian.org/doc/manuals/debian-handbook/network-infrastructure.zh-cn.html>,
<https://www.debian.org/doc/manuals/debian-handbook/sect.virtual-private-network.zh-cn.html>,
<https://www.debian.org/doc/manuals/debian-handbook/sect.x509-cert.zh-cn.html>

**tap、tun、虚拟网卡、网桥**:
[重拾 Linux 网络（一）：iptables                                    ](https://pandaychen.github.io/2023/08/01/A-IPTABLES-REVIEW),
[重拾 Linux 网络（二）：网卡 / 虚拟网卡、tap/tun 那些事](https://pandaychen.github.io/2023/08/02/NETWORK-REVIEW),
[理解Linux虚拟网卡设备tun/tap的一切](https://www.junmajinlong.com/virtual/network/all_about_tun_tap/index.html),

<https://mangohost.net/blog/tap-vs-tun-a-comprehensive-guide>

<https://docs.redhat.com/en/documentation/red_hat_enterprise_linux/7/html/networking_guide/sec-configuring_ip_networking_with_ip_commands>

### DNS
Command: `nslookup, dig`:

[Debian上使用Dnsmasq设置本地DNS](https://cn.linux-console.net/?p=30658),
[Debian修改DNS服务器](https://www.cnblogs.com/edgecode/p/Debian11-Change-DNS-Server.html)

### X11
X11 GUI: Putty + Xming

[error: X11 forwarding request failed on channel 0](https://linux.cn/article-4014-1.html)

<https://serverfault.com/questions/422908/how-can-i-prevent-the-warning-no-xauth-data-using-fake-authentication-data-for>,
<https://askubuntu.com/questions/1040108/ssh-uses-fake-authentication-for-x11-forwarding>,

<https://x410.dev>,
<https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html>

<https://zhuanlan.zhihu.com/p/66075449>,
<https://zhuanlan.zhihu.com/p/157479678>

<https://some-natalie.dev/blog/ssh-x11-forwarding>

<https://mobaxterm.mobatek.net>

<https://locall.host/windows-ssh-with-x11-forwarding/?expand_article=1>

<https://bytebitebit.com/operating-system/linux/how-to-set-display-variable-in-linux>

## REMOTE

### RDP
`mstsc` is command for connecting to remote machine. should enable remote feature in windows first

`vncserver` is command for enabling deamon in server side

<https://www.realvnc.com>

### SSH
`ssh` and `scp` are command that can be used between different system. should enable ssh-server in windows first. should install openssh-server in linux first.

[win10 开启ssh server服务 远程登录](https://blog.csdn.net/weixin_43064185/article/details/90080815)

[Key-based authentication in OpenSSH for Windows](https://learn.microsoft.com/en-us/windows-server/administration/openssh/openssh_keymanagement): `authorized_keys, administrators_authorized_keys`,
[Get started with OpenSSH for Windows           ](https://learn.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse)

[Linux系统SSH客户端断开后保持进程继续运行配置方法](https://help.aliyun.com/document_detail/42523.html)

[保持ssh session在断开连接后保持运行的五种方法](https://blog.csdn.net/qq_34769162/article/details/107948168)

[xvfb初步探究](https://blog.csdn.net/span76/article/details/11473315)

<https://www.openssh.com>

<https://github.com/openssh/openssh-portable>,
<https://github.com/PowerShell/openssh-portable>

scp -P
ssh -p -l

[warning: agent returned different signature type ssh-rsa (expected rsa-sha2-512) when key registered with ssh-agent](https://github.com/PowerShell/Win32-OpenSSH/issues/1551): 使用ssh -V发现笔记本是8x的ssh没有这个问题，台式机是7x的有问题。这个问题导致了不能免密码登录。可以用git里面的ssh，试过没有问题。

<https://www.baeldung.com/linux/ssh-authentication-methods>,
<https://www.ssh.com/academy/ssh/host-key>,
<https://www.ruanyifeng.com/blog/2020/07/ssh-certificate.html>,
<https://unix.stackexchange.com/questions/102502/meaning-of-connection-closed-by-xxx-preauth-in-sshd-logs>

### [VT100](http://vt100.net)

<https://invisible-island.net/xterm/ctlseqs/ctlseqs.html>

LINUX VT100:
<https://man7.org/linux/man-pages/man4/console_codes.4.html>

WINDOWS VT100:
<https://learn.microsoft.com/en-us/windows/console/classic-vs-vt>,
<https://learn.microsoft.com/en-us/windows/console/console-functions>,
<https://learn.microsoft.com/en-us/windows/console/console-virtual-terminal-sequences>,
<https://learn.microsoft.com/en-us/windows/console/ecosystem-roadmap>,
<https://learn.microsoft.com/en-us/windows/console/setconsoletextattribute>,
<https://learn.microsoft.com/en-us/windows/console/using-the-high-level-input-and-output-functions>

Some basic knowledge:
[SecureCRT中的终端选择VT100 VT102 VT200 Xterm linux Vshell](https://zhidao.baidu.com/question/352524515.html),
[什么是vt100？ -技术百科的定义](https://cn.theastrologypage.com/vt100)

NOTEs:  
Linux对VT100支持较好，其中python在linux上print就可以使用，但windows则不可以。  
Windows对VT100支持不太好，但WIN11开始改进很多，其中使用`type`可以输出包含VT100编码的文本，但如果more来分行的则会被影响。 Powershell运行python时，print打印支持VT100，这个可以做为WIN10的WA。

### CREDENTIAL

[usingcurl-netrc](https://github.com/chinanf-boy/everything-curl-zh/blob/master/book/usingcurl-netrc.zh.md)

[.netrc File Format for TCP/IP](https://www.ibm.com/docs/en/aix/7.3?topic=formats-netrc-file-format-tcpip)

[linux 密码记录文件 .netrc 简介](https://blog.csdn.net/whatday/article/details/106000186): netrc can be used for git, curl, ftp

[用户配置脚本文件.netrc](https://kekxv.github.io/2021/01/06/User configuration script file .netrc)

[github添加ToKen到本地并写入netrc实现自动登录](https://blog.csdn.net/bjbz_cxy/article/details/121851002)

[FTP初始化文件.netrc使用技巧](http://www.360doc.com/content/15/0827/14/1106320_495171593.shtml)

[Git-如何在Windows上使用.netrc文件保存用户和密码](https://qastack.cn/programming/6031214/git-how-to-use-netrc-file-on-windows-to-save-user-and-password)

[Git-Credential-Manager-for-Windows](https://github.com/Microsoft/Git-Credential-Manager-for-Windows)

[github token by git and netrc](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens)

### [PUTTY](https://putty.org)

[Ubuntu 18.04 LTS 使用xrdp远程桌面配置说明](https://www.cnblogs.com/varden/p/13954575.html),
[Can't connect to xrdp as normal user, connecting as root is fine](https://unix.stackexchange.com/questions/629505),
[xrdp方式windows 10连接ubuntu 18.04](https://zhuanlan.zhihu.com/p/40937988),
[Issues with xRDP and Ubuntu 18.04.2 – How to fix it](http://c-nergy.be/blog/?p=13390),
[windows用xrdp方式远程桌面连接ubuntu](https://blog.csdn.net/devil6636252/article/details/109616851),
[使用 Windows 远程 Linux 主机 @20210130](https://blog.csdn.net/u013670453/article/details/113423956)

[wpa_supplicant 常用操作及其wpa_cli无法运行的原因Could not connect to wpa_supplicant](https://blog.csdn.net/qq_32348883/article/details/123156401),
[systemctl开机启动wpa_supplicant](https://blog.csdn.net/u010049696/article/details/48765999)

[ngrok的使用(超详细)](https://blog.csdn.net/liunianqingshi/article/details/108049441)

[最佳 Linux 远程桌面客户端 | Linux 中国](https://zhuanlan.zhihu.com/p/586858767),
[Remmina](https://remmina.org),
[Best RDP (Remote Desktop) Clients for Linux](https://www.tecmint.com/best-linux-rdp-remote-desktop-clients)

### OTHER REMOTE SOLUTION
1. TEAMVIEWER: TeamViewer user profile can set which machine are login, free user can only login two machine

## VERSIONCONTROL

### [GIT](https://git-scm.com)
GIT官网的说明文档可能会比bending的落后

[Send a collection of patches as emails](https://git-scm.com/docs/git-send-email)

git添加submodule时，会创建一个160000属性的commit文件，此commit对应submodule对应的commit。commit之前可以用`git diff --cached`查看此文件存在，commit之后可用`git ls-tree`查看此文件存在。此commit文件无法用`git cat-file`查看。
其中的.gitmodule文件也非常重要，缺少会导致`git submodule`命令无法正常运行。
submodule必须到对应子目录才能使用git命令查看其内容。

`git config core.logpaths true`解决windows长文件名

<https://docs.github.com/en/rest/pulls>

### MIDDLEWARE

### [GITHUB](https://github.com)

<https://docs.github.com>, <https://github.com>, <https://github.io>, <https://github.dev>, <https://github.com/settings/tokens>

[怎样通过GitHub REST API v3获得某个项目的所有issue](https://blog.csdn.net/qysh123/article/details/79626894)


path(pulls, compare, branches, commits, tree, blob) in github:
<https://github.com/tianocore/edk2/pulls>,
<https://github.com/tianocore/edk2/pulls/kuqin12>,
<https://github.com/tianocore/edk2/compare/8750141...03a5c1e>,
<https://github.com/tianocore/edk2/branches>,
<https://github.com/tianocore/edk2/commits/master>,
<https://github.com/tianocore/edk2/commits/master/ArmPkg>,
<https://github.com/tianocore/edk2/tree/master>,
<https://github.com/tianocore/edk2/blob/master/ArmPkg/ArmPkg.dec>

fork in github:
<https://github.com/tianocore/edk2/forks>,
<https://github.com/tianocore/edk2/network/members>

## BUGTRACKER

### EIP

### BUGZILLA

### JIRA

## SEARCH

[搜网](http://sowang.com)

[Bing Search Operators Cheat Sheet](https://www.sidegains.com/search-engines/bing-search-operators-cheat-sheet)

## CAD

### LEGO

[LEGO Digital Designer即将下线，将被BrickLink Studio正式取代](https://zhuanlan.zhihu.com/p/456804889), <https://www.bricklink.com>

## BROWSER

[测网速](https://www.speedtest.cn)

[运营商测速猫腻](https://zhuanlan.zhihu.com/p/82105234)

## PDA

[华为手机“定时播报日程安排”提醒](https://zhuanlan.zhihu.com/p/409690217)

## EDA

## TIME

<https://24timezones.com/#/map>

### CALENDAR

1. <https://blog.csdn.net/gitblog_00026/article/details/139210730>, <https://gitcode.com/gh_mirrors/cal/Calendar.js>, <https://calendar-js.com/download.html>
2. <https://blog.csdn.net/gitblog_00070/article/details/139517876>, <https://gitcode.com/gh_mirrors/op/open-web-calendar>

## COMMUNICATION

### WECHAT

[微信的聊天记录为什么总是自动消失](https://zhidao.baidu.com/question/814527655836741732/answer/2865264035)

## SECURITY

1. [Authy](https://mobile.softpedia.com/apk/authy)
2. <https://keepass.info>, <https://github.com/PhilippC/keepass2android/releases>
3. [Kerberos安装教程与命令详解](https://zcs2312.blog.csdn.net/article/details/135245018)
4. [Kerberos中常用命令](https://blog.csdn.net/weixin_38233104/article/details/130912374): `krb5-user, libkrb5-dev`
5. <https://wentzwu.com/2021/02/01/active-directory-domains-and-kerberos-reals>
6. <https://web.mit.edu/kerberos/kfw-4.1/kfw-4.1/kfw-4.1-help/html/kerberos_terminology.htm>
7. <https://kb.mit.edu/confluence/display/glossary/Kerberos>
8. [linux服务器加入AD域](https://www.cnblogs.com/zhangmingda/p/13994027.html)
9. [Kerberos基本原理、安装部署及用法](https://www.cnblogs.com/swordfall/p/12009716.html)
10. [windows域认证Kerberos详解](https://blog.csdn.net/wy_97/article/details/87649262)
11. [Windows域权限维持](https://blog.csdn.net/qq_55202378/article/details/141124647)
12. [Linux加入Windows域](https://blog.csdn.net/m0_57695646/article/details/122038213)

## BOOT

[带EFI支持的GRUB2安装全记录](https://www.cnblogs.com/ricksteves/p/11623681.html)

## PACKAGE MANAGEMENT

`rpm, yum, dpkg, apt, npm, pip`

<https://guozh.net/google-play-apk-download>, <apkcombo.com>, <apkpure.com>

## FINANCE

### Gnucash

1. <https://github.com/codinguser/gnucash-android>

## FILE MANAGER

### VHD

1. [VHD更新命令](https://blog.csdn.net/weixin_34270865/article/details/94530997)

## Graph Theory

1. <https://cytoscape.org>: can import file with `.graphml` prefix

## Virtualization
[**XEN VMWARE QEMU OVMF KVM SIMICS HYPERVISOR**](https://wiki.xenproject.org/wiki/OVMF)

[创建镜像image、启动容器container、删除容器、进入容器](https://blog.csdn.net/pearl8899/article/details/113757377),
[Linux 容器化技术详解](https://blog.csdn.net/daocaokafei/article/details/118075369),
[Docker](https://docker-practice.github.io/zh-cn/basic_concept/image.html),
[Debian install Xen](https://www.mryunwei.com/254056.html),
[VPS超售](https://blog.csdn.net/bingbob/article/details/105803431),
[VPS超售](https://www.evec.cc/2019/02/06/vpsovercommit)

[KVM - Kernel based Virtual Machine](https://wiki.archlinux.org/title/KVM),
[QEMU                              ](https://wiki.archlinux.org/title/QEMU)

[KVM vs Xen](https://www.techtarget.com/searchitoperations/tip/Xen-vs-KVM-What-are-the-differences),
[QEMU vs XEN](https://superuser.com/questions/170768/difference-between-qemu-kvm-and-xen-virt-manager),
[OVMF](https://cloud-atlas.readthedocs.io/zh_CN/latest/kvm/iommu/ovmf.html),
[UEFI / OVMF](https://wiki.ubuntu.com/UEFI/OVMF),
[Compare between Xen KVM](https://www.researchgate.net/figure/A-comparison-chart-between-Xen-KVM-VirtualBox-and-VMWare-ESX_fig2_224257050),
[Xen KVM Qemu](https://blog.csdn.net/ysbj123/article/details/51166343),
[KVM XEN](https://ww.cnblogs.com/qinlulu/p/13204849.html),
[QEMU vs KVM](https://www.linuxmi.com/qemu-vs-kvm.html)

[linux下挂载VHD等虚拟磁盘文件](https://www.cnblogs.com/oloroso/p/6385398.html)

### [QEMU](https://www.qemu.org)
Docs:
[usb   ](https://www.qemu.org/docs/master/system/devices/usb.html),
[images](https://www.qemu.org/docs/master/system/images.html),
[gdb   ](https://www.qemu.org/docs/master/system/gdb.html),
[xen   ](https://www.qemu.org/docs/master/system/i386/xen.html)

Repos:
<https://github.com/qemu/qemu>

Refs:
1. <https://wiki.debian.org/Cloud>, <https://wiki.debian.org/ThomasChung/CloudImage>, <https://wiki.debian.org/Cloud/SystemsComparison>
2. <https://leux.cc/doc/Debian官方qcow2镜像修改root密码.html>

3. <https://cloudinit.readthedocs.io/en/latest/tutorial/qemu.html>
4. <https://cloudinit.readthedocs.io/en/latest/reference/network-config.html>
5. <https://cloudinit.readthedocs.io/en/latest/reference/datasources/nocloud.html>
6. <https://cloudinit.readthedocs.io/en/latest/reference/modules.html#users-and-groups>

[qemu fat](https://ww.emaculation.com/forum/viewtopic.php),
[qemu drive parameter](https://www.cnblogs.com/honpey/p/8505550.html),
[QEMU img](https://www.cnblogs.com/wyzhou/p/9602606.html),
[qemu - img convert](https://blog.csdn.net/allway2/article/details/122213307),
[Converting image format](https://docs.openstack.org/image-guide/convert-images.html),
[QEMU Start](https://blog.csdn.net/fontthrone/article/details/104157859),

<https://wiki.qemu.org/Feature/Q35>

[Windows下QEMU虚拟化探索](https://www.cnblogs.com/suzhoulaowang/p/18195323)
[UEFI启动原理及qemu虚拟化中使用](https://blog.csdn.net/weixin_43269452/article/details/139861998)
<https://pve.proxmox.com/pve-docs/pve-admin-guide.html>

## STREAM
[本地搭建RTMP服务](https://blog.csdn.net/yelin042/article/details/106448111),
[直播推流操作手册](https://blog.csdn.net/lovebird321/article/details/105532759),
 
[无人值守直播工具](https://github.com/withsalt/BilibiliLiveTools)

[OBS定时自动推流设置](https://www.bilibili.com/read/cv19838044)

[7×24无人值守直播推流软件开发实战](https://blog.csdn.net/blogtime/article/details/133862103)

[7x24小时自动推流服务器搭建](https://www.jianshu.com/p/f5a53bdbf2a9)

<https://www.obsproject.com.cn/obs/265.html>

<https://developers.weixin.qq.com/miniprogram/dev>,
<https://developers.weixin.qq.com/community/develop>

## COMPRESS
[Linux下常用压缩解压命令和压缩比率对比](https://blog.csdn.net/buknow/article/details/115053065)

## HOTKEYS
1. `CTRL + TAB/PAGEUP/PAGEDOWN`: Switch pages in EDGE/CHROME explorer

## GUI
1. <https://github.com/slint-ui/slint/tree/master/examples/uefi-demo>
2. <https://github.com/google/skia>
3. [Skia全面解读](https://endlessyoung.github.io/Blog_/Android/Skia.html)
4. [Skia编译及踩坑实践](https://helloworld.net/p/8339648946)
5. [Skia VS Impeller](https://segmentfault.com/a/1190000045115269)
6. [Skia Overview and API Reference](https://zhuanlan.zhihu.com/p/157587058)

## SECURITY
1. [MSI UEFI私钥泄露事件简要分析](https://www.secrss.com/articles/54636)

# SYSTEM SOFTWARE

## OS
Operation System are system software, include windows, linux.  
system software vendor include microsoft, ubuntu, debian, centos, redhat, etc  
Vendor websites are <microsoft.com>, <ubuntu.com>, <debian.org>, <centos.org>, <redhat.com>
linux kernel is very important, the website is <kernel.org>

### WINDOWS

windows设置里面，账户选项卡，账户信息里面，账户设置里选择改用本地设置可以在本地与微软账户切换。
在控制面板里面，可以删除保存的密码，这样浏览器就不会自动登录。

[win10搜索框的热门搜索怎么关闭?](https://www.zhihu.com/question/563437571)

[windows10如何关闭搜索功能中展示的热门搜索？](https://answers.microsoft.com/zh-hans/windows/forum/all/windows10%e5%a6%82%e4%bd%95%e5%85%b3%e9%97%ad/4c89657e-f0c7-45f9-9908-3b1657aa76e0)

[win11微软拼音输入法选字候选框无法显示](https://zhuanlan.zhihu.com/p/430128136)

[“磁盘空间不足”错误](https://blog.csdn.net/weixin_36086032/article/details/113327035),
[临时文件夹已满或不能访问](https://blog.csdn.net/qq_48081868/article/details/132097740)

<https://learn.microsoft.com>

<https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/systeminfo>
<https://learn.microsoft.com/en-us/windows-hardware/drivers/devtest/pnputil-examples>
<https://learn.microsoft.com/en-us/windows-hardware/drivers/devtest/certmgr>

<https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/tasklist>

<https://learn.microsoft.com/zh-cn/sysinternals/downloads/bginfo>

<https://docs.microsoft.com/en-us/windows-hardware/drivers/devtest/boot-options-in-windows>

<https://developer.microsoft.com/en-us/graph/quick-start>,
<https://learn.microsoft.com/en-us/graph/overview>

[win10 挂载NFS](https://blog.csdn.net/qq_34158598/article/details/81976063)

#### Native Command Line
| Name                                                                                                    | Description                                      |
|---------------------------------------------------------------------------------------------------------|--------------------------------------------------|
| [`type`](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/type)         | Display contents of file, similar as linux `cat` |
| [`msinfo32`](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/msinfo32) | Comprehensive view of the hardware               |
| [`msconfig`](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands)          | Change the boot option                           |
| [`bootsect`](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands)          | NA                                               |
| [`bcdedit`](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/bcdedit)   | Managing BCD store                               |
| [`bootcfg`](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/bootcfg)   | Change Boot.ini                                  |
| [`cd`](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/cd)             | Change directory                                 |
| [`dir`](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/dir)           | Displays a list of a files and subdirectories    |
| [`whoami`](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/whoami)     | Display user name                                |
| [`hostname`](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/hostname) | Display host name                                |

### LINUX

<https://www.debian.org/distrib/packages>,
<https://packages.debian.org/bookworm/easy-rsa>,
<https://packages.ubuntu.com>,
<https://centos.org>,
<https://www.suse.com>,
<https://www.redhat.com>

[Linux文件系统详解](http://c.biancheng.net/view/880.html)

<https://docs.kernel.org>

<https://docs.centos.org/en-US/8-docs/managing-userspace-components/assembly_finding-rhel-8-content>

<https://centos.pkgs.org/8-stream/centos-baseos-x86_64/shim-x64-15-15.el8_2.x86_64.rpm.html>

<https://packages.debian.org/bookworm/shim-unsigned>

<https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html/networking_guide/ch-consistent_network_device_naming>

[Linux守护进程的启动方法](https://www.ruanyifeng.com/blog/2016/02/linux-daemon.html),
[Systemd入门教程        ](https://ruanyifeng.com/blog/2016/03/systemd-tutorial-commands.html),
[init进程详解](https://blog.csdn.net/hxpjava1/article/details/79825674),
[/etc/profile详解](https://blog.csdn.net/hao745580264_dawei/article/details/140341667)

[如何编写一个systemd service](https://segmentfault.com/a/1190000014740871): <https://systemd.io>, <https://github.com/systemd/systemd>, <https://www.freedesktop.org/wiki/Software/systemd>, <https://packages.debian.org/bookworm/systemd-sysv>

[Linux内核为什么会发生soft lockup？](https://blog.csdn.net/21cnbao/article/details/108250786)

[shell脚本无法使用source命令的原因与解决方法](https://www.cnblogs.com/luego/p/11684311.html)

<https://unix.stackexchange.com/questions/68079/mount-cifs-network-drive-write-permissions-and-chown>

<https://cdimage.debian.org/cdimage/cloud/sid/daily>, <https://cdimage.ubuntu.com/releases>

`env|grep -i proxy`: `/etc/environment`, `no_proxy/NO_PROXY`
`/etc/profile`

[cp复制软连接](https://www.cnblogs.com/chentiao/p/17363300.html)

[Linux NFS文件共享](https://blog.csdn.net/Dark_Tk/article/details/114100517)

#### Native Command Line
| Name                                                      | Description                                         |
|-----------------------------------------------------------|-----------------------------------------------------|
| [`cat`](https://packages.debian.org/buster/coreutils)     | Display contents of file, similar as windows `type` |
| [`dir`](https://packages.debian.org/buster/coreutils)     | Displays a list of a files and subdirectories       |
| [`ls`](https://packages.debian.org/buster/coreutils)      | Displays a list of a files and subdirectories       |
| [`whoami`](https://packages.debian.org/buster/coreutils)  | Display user name                                   |
| [`hostname`](https://packages.debian.org/buster/hostname) | Display host name                                   |
| [`sh`](https://packages.debian.org/buster/dash)           | compatible with posix shell                         |
| [`bash`](https://packages.debian.org/buster/bash)         | shell interpreter                                   |
| [`type`](https://packages.debian.org/buster/dash)         | interpretion as a commnd name, shell builtin        |
| [`cd`](https://packages.debian.org/buster/dash)           | Change directory, shell builtin                     |
