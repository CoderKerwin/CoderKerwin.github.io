# software

## EDITOR

### VIM

<https://www.vim.org>, <https://github.com/vim>, <https://github.com/neovim/neovim>

<https://github.com/termux/termux-app>, <https://f-droid.org/en/packages/com.termux>

<https://github.com/jackpal/Android-Terminal-Emulator>

<https://github.com/shiftrot/droidvim>

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
代码浏览

### OPENGROK
[OPENGROK](https://opengrok.github.io)

### CODE-SERVER
[CODE-SERVER](https://github.com/coder/code-server)

### CSCOPE
[CSCOPE](https://github.com/yifengyou/cscope)
[CSCOPE](https://github.com/Hyeonykim/cscope)
[CSCOPE](https://github.com/youyuanwu/cscope)
[CSCOPE](https://github.com/Smattr/clink)

## ANALYSIS
静态分析

### COVERITY

### KLOCKWORK

## UNITTEST
单元测试：以数据为中心进行测试

[OpenCppCoverage](https://github.com/OpenCppCoverage/OpenCppCoverage)
[C++开源代码覆盖率工具OpenCppCoverage介绍(Windows)](https://www.cnblogs.com/coderzh/p/OpenCppCoverage.html)
[GCOV使用    ](https://blog.csdn.net/lishenglong666/article/details/8056777)
[gcov使用小节](https://blog.csdn.net/weixin_41910194/article/details/80759473)

### CMOCKA

## COMPILER

### ASSEMBLER

#### NASM

### C/C++ COMPILER

#### MSVC

[MSVC编译器参考](https://learn.microsoft.com/zh-cn/cpp/build/reference/compiling-a-c-cpp-program?view=msvc-170)

Zi, /debug

#### GCC

[GNU Compiler Collection          ](https://gcc.gnu.org)
[Options That Control Optimization](https://gcc.gnu.org/onlinedocs/gcc/Optimize-Options.html)

[GCC基本使用](https://zhuanlan.zhihu.com/p/404682058)

-g

#### CLANG

#### KEIL

[stc-isp安装教程win11_stcisp安装教程win11](https://www.keil345.com/keil/108528.html)

[STC-ISP单片机烧录软件](http://www.i5wz.com/soft/bckf/11509.html)

## JAVA COMPILER

Bing: OpenJDK download
<https://jdk.java.net/archive>
<https://download.java.net/java/GA/jdk11/9/GPL/openjdk-11.0.2_windows-x64_bin.zip>

### OPENJDK

## DISASSEMBER
readelf, nm, objdump, dumpbin

### DUMPBIN

### OBJDUMP

### NM

### IDA

## DEBUGGER

### GDB
[Options for Debugging Your Program](https://gcc.gnu.org/onlinedocs/gcc/Debugging-Options.html)

[gdb调试用法](https://www.cnblogs.com/ims-/p/10529393.html)

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
[Approving a pull request with required reviews](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/approving-a-pull-request-with-required-reviews)
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

[TeamCity](https://www.jetbrains.com/teamcity)
[TeamCity VS Jenkins：选择正确的CI / CD工具](https://cloud.tencent.com/developer/article/1664894)
[谁才是世界上最好的 CI/CD 工具？](https://zhuanlan.zhihu.com/p/67805669)
[Azure DevOps](https://azure.microsoft.com/en-us/products/devops)

## NETWORK
`systemctl status networking`, `/etc/systemd/system/network*`, `/lib/systemd/system/network*`, `/sbin/ifup`, `/etc/network/if-up.d`, `/etc/network/interfaces`

`/lib/systemd/system/networking.service`会调用`ifup`，`ifup`会调用`/etc/network/if-up.d/wpasupplicant`，但因为`/etc/network/interfaces`里面没有wpa相关配置，所以wpasupplicant只跑了`start()`就退出了。  
`networking.service`在`wpa_supplicant.service`之前运行，所以networking由于wpa为准备好无法正常配置dhcp。  
当前暂时改了`/etc/network/interfaces`与`wpasupplicant`两个文件解决debian无法配置开机自动配置wifi问题。

`/sbin/init`是指向`/sbin/systemd`的软链接

### VPS
<https://www.vpstop.cn>

### FRP
[frp内网穿透](https://itlanyan.com/frp-tunnel-tutorial)
<https://github.com/fatedier/frp/releases>

### PROXY
[Linux配置成代理服务器](https://www.cnblogs.com/caopeng/p/17909476.html)

### OPENVPN
<https://ubuntu.com/server/docs/how-to-install-and-use-openvpn>,
<https://documentation.ubuntu.com/server/how-to/security/install-openvpn>,
<https://github.com/openvpn>,
<https://openvpn.net/community>,
<https://www.doncaprio.com/how-to-create-a-personal-vpn-openvpn-on-your-vps>,
[OpenVPN配置代理路由实现局部代理](https://www.luisimon.com/2020/04/25/318),
[手把手教你搭建OpenVPN](https://blog.admin4j.com/linux/vpn),
[openvpn配置实现服务器代理上网](https://blog.csdn.net/java_linux_dev/article/details/135879838),
[搭建OpenVpn实现服务器代理上网](https://blog.csdn.net/weixin_44105868/article/details/139463173)

**tap、tun、虚拟网卡、网桥**:
[重拾 Linux 网络（一）：iptables                                    ](https://pandaychen.github.io/2023/08/01/A-IPTABLES-REVIEW),
[重拾 Linux 网络（二）：网卡 / 虚拟网卡、tap/tun 那些事](https://pandaychen.github.io/2023/08/02/NETWORK-REVIEW),

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

## REMOTE

### RDP
`mstsc` is command for connecting to remote machine. should enable remote feature in windows first

`vncserver` is command for enabling deamon in server side

<https://www.realvnc.com>

### SSH
`ssh` and `scp` are command that can be used between different system. should enable ssh-server in windows first. should install openssh-server in linux first.

[win10 开启ssh server服务 远程登录](https://blog.csdn.net/weixin_43064185/article/details/90080815)

[Key-based authentication in OpenSSH for Windows](https://learn.microsoft.com/en-us/windows-server/administration/openssh/openssh_keymanagement): `authorized_keys, administrators_authorized_keys`
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

[Ubuntu 18.04 LTS 使用xrdp远程桌面配置说明](https://www.cnblogs.com/varden/p/13954575.html)
[Can't connect to xrdp as normal user, connecting as root is fine](https://unix.stackexchange.com/questions/629505)
[xrdp方式windows 10连接ubuntu 18.04](https://zhuanlan.zhihu.com/p/40937988)
[Issues with xRDP and Ubuntu 18.04.2 – How to fix it](http://c-nergy.be/blog/?p=13390)
[windows用xrdp方式远程桌面连接ubuntu](https://blog.csdn.net/devil6636252/article/details/109616851)
[使用 Windows 远程 Linux 主机 @20210130](https://blog.csdn.net/u013670453/article/details/113423956)

[wpa_supplicant 常用操作及其wpa_cli无法运行的原因Could not connect to wpa_supplicant](https://blog.csdn.net/qq_32348883/article/details/123156401)
[systemctl开机启动wpa_supplicant](https://blog.csdn.net/u010049696/article/details/48765999)

[ngrok的使用(超详细)](https://blog.csdn.net/liunianqingshi/article/details/108049441)

[最佳 Linux 远程桌面客户端 | Linux 中国](https://zhuanlan.zhihu.com/p/586858767)
[Remmina](https://remmina.org)
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

<https://learn.microsoft.com>

<https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/systeminfo>
<https://learn.microsoft.com/en-us/windows-hardware/drivers/devtest/pnputil-examples>
<https://learn.microsoft.com/en-us/windows-hardware/drivers/devtest/certmgr>

<https://docs.microsoft.com/en-us/windows-hardware/drivers/devtest/boot-options-in-windows>

<https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/tasklist>

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

## BUGTRACKER

### EIP

### BUGZILLA
缺陷管理

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

## COMMUNICATION

### WECHAT

[微信的聊天记录为什么总是自动消失](https://zhidao.baidu.com/question/814527655836741732/answer/2865264035)

## SECURITY

1. [Authy](https://mobile.softpedia.com/apk/authy)
2. <https://keepass.info>, <https://github.com/PhilippC/keepass2android/releases>

## BOOT

[带EFI支持的GRUB2安装全记录](https://www.cnblogs.com/ricksteves/p/11623681.html)

## PACKAGE MANAGEMENT

`rpm, yum, dpkg, apt, npm, pip`

## FINANCE

### Gnucash

1. <https://github.com/codinguser/gnucash-android>

## FILE MANAGER

### VHD

1. [VHD更新命令](https://blog.csdn.net/weixin_34270865/article/details/94530997)

## Graph Theory

1. <https://cytoscape.org>: can import file with `.graphml` prefix
