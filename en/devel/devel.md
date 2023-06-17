这里涉及开发全生命周期内容，包括规范与工具。
全生命周期包括：需求分析、可行性分析、系统设计、编码、测试、维护
遇到问题可以先在社区或项目问题描述里看看：是否是已知问题，是否有临时方法。

操作系统、编译器、数据库
编程语言、数据结构与算法

[数据结构与算法、计算机网络、操作系统、设计模式](https://blog.csdn.net/weixin_46698891/article/details/113814822)

## ISA

### X86

[Intel SDM](https://www.intel.com/content/www/us/en/developer/articles/technical/intel-sdm.html)

[Amd APM](https://www.amd.com/en/support/tech-docs/amd64-architecture-programmers-manual-volumes-1-5)

### ARM

### RISCV

[RISC-V](https://riscv.org)

## APPLICATION

[C语言教你怎么改变字体颜色](https://blog.csdn.net/qq_31975227/article/details/51758461): dropped by windows

## HARDWARE

[Open Compute Project](https://www.opencompute.org)

[量子兔 alphapi 硬件拆解分析 尝试自己从头写库](https://blog.csdn.net/jd3096/article/details/127000637)

[AlphaPi](https://github.com/eggfly/AlphaPi)

[Raspberry Pi](https://www.raspberrypi.com)

## FIRMWARE

https://www.osfc.io
https://www.opencompute.org
https://www.coreboot.org
https://www.trustedfirmware.org
https://www.linuxboot.org

https://github.com/hardenedlinux
https://github.com/openbmc/docs
https://github.com/oreboot/oreboot
https://github.com/hardenedvault/vaultboot
https://slimbootloader.github.io
https://system-transparency.org
https://www.tianocore.org
https://u-bmc.org
https://www.denx.de/wiki/U-Boot
https://u-root.org

### TIANOCORE
  TIANOCORE项目学习路径：
  [UEFI and PI and ACPI spec](https://uefi.org)     ：UEFI与ACPI相关规范
  https://www.tianocore.org                         ：website
  https://github.com/tianocore/edk2                 ：主要的edk2代码实现，其中包含OVMF测试环境
  https://github.com/tianocore/edk2-platforms       ：主要基于edk2框架的实现平台
  https://github.com/tianocore/edk2-staging         ：包含UNDI等POC的代码，在不同分支上
  https://github.com/tianocore/edk2-libc            ：包含最新的python3的移植
  https://github.com/tianocore/tianocore.github.io  ：网页https://www.tianocore.org的源头，目录一一对应。这里的wiki是另外仓库，需要特别注意，并且其中有很多有用信息
  https://github.com/tianocore-docs                 ：edk2相关文档仓库
  https://github.com/tianocore-training             ：edk2相关培训资料仓库
  https://bugzilla.tianocore.org                    ：bug与feature跟踪系统
  https://edk2.groups.io                            ：maillist讨论

  [FWTS](https://uefi.org/sites/default/files/resources/fwts_uefi_0920_2013.pdf)

  https://bsdio.com/edk2/docs/master/index.html

  No matter Ppi or Protocol, there can be installed many same instance. It is like class and instance.

  TIANOCORE文档采用了github.io与gitbook.io两种方式，关于文档化的Wiki参考下面两个文档。当前所有EDK II文档都转到tianocore-docs仓库管理。关于EDK II的Training则转到tianocore-training仓库管理
  [EDK II Draft Specification](https://github.com/tianocore/tianocore.github.io/wiki/EDK-II-Draft-Specification)
  [EDK II Documentation      ](https://github.com/tianocore/tianocore.github.io/wiki/EDK-II-Documentation)
  
  关于文档具体例子如下。看tianocore-docs仓库有个gh-pages分支估计就是静态网页所保存的位置，目录规则应该使具体库名(这里是edk2-BuildSpecification)加上gh-pages分支对应路径名(比如此处的draft与release-1.28)加上具体路径名(如1_introduction)。
  这里特别注意的是只有拥有gh-pages分支的仓库才可以访问且必须带有gh-pages分支的目录，比如draft或release-1.28
  关于gh-pages可以参考https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site，其中<code>https://<user>.github.io/<repository>/about/contact-us.html</code>就是github网页的路径规则。
  [EDK II Build Specification](https://tianocore-docs.github.io/edk2-BuildSpecification/draft)
  [EDK II Build Specification](https://tianocore-docs.github.io/edk2-BuildSpecification/release-1.28)
  
  另外看似之前也用了gitbook来产生文档但后来不用了，这里提供下参考。除了中间仓库名不是很清楚，具体路径名应该与tianocore-docs类似
  另外值得一说的是：tianocore-docs.github.io对应的www.gitbook.com/read/book/edk2-docs/edk-ii-build-specification需要登录，可以将路径直接改为edk2-docs.gitbook.io/edk-ii-build-specification，虽然这样子不能下载诸如pdf与emobi版本
  [EDK II Build Specification](https://edk2-docs.gitbook.io/edk-ii-build-specification)
  
  另外一个是关于tianocore-training的，这个有空时看看，暂时感觉其中文档没啥用处。

  [EDK II Code Formatting](https://github.com/tianocore/tianocore.github.io/wiki/EDK-II-Code-Formatting)里面有Uncrustify的详细介绍

  [EDK II Uncrustify fork repository](https://dev.azure.com/projectmu/Uncrustify)

  [Uncrustify executables are built from this fork source code and published as Nuget packages](https://dev.azure.com/projectmu/Uncrustify/_packaging?_a=feed&feed=mu_uncrustify)这个Nuget直接用7Z打开取里面exe就好了

  [Code Style](https://github.com/tianocore/tianocore.github.io/wiki/Code-Style)

## SOFTWARE

### MIDDLEWARE

#### LIBRARY

##### STDLIB

## PROGRAMMING LANGUAGE

### C/C++
[C++知识回顾之__stdcall、__cdecl和__fastcall三者的区别__ end__](https://www.cnblogs.com/yejianyong/p/7506465.html): C calling convention
[C的隐式类型转换](https://www.veaxen.com/c的隐式类型转换.html)
[C语言32个关键字-最详解释                      ](https://blog.csdn.net/qq_38972634/article/details/108398953)

[open-source formatting library providing a fast and safe alternative to C stdio and C++ iostreams](https://fmt.dev)

## Builder
软件构建：ant/nant/gradle/cmake/make/nmake/msbuild

### MAKE

### NMAKE

### MSBUILD

### ANT

### GRADLE

### CMAKE

### EDK2-BASETOOLS

## COMPILER

### C/C++ COMPILER
编译工具：MSVC、GCC、CLANG

#### MSVC

/Zi, /debug

#### GCC

-g

#### CLANG

### ASSEMBLER

#### NASM

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

gdb命令```b/bt/c/d/h/i/n/p/q/r/s/x/mem/display```，详细如下
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

symbol-file : load symbol. <code>symbol-file -o offset FILE</code>

mem         : show memory
display     : display variable
disassemble : disassemble. /r /s modifier
list        : list source of function or line

[GDB用法详解](https://www.cnblogs.com/lvdongjie/p/8994092.html)

### WINDBG

windbg命令```bp/d/g/gc/k/p/q/r/t/x```，详细如下
bp  : break
d   : display memory.
dt  : display type
dv  : display local variable
dx  : display C++ expression. dx -r1 (*((Test!_EFI_PLATFORM_INFO *)0x0))
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

#### DBH

dbh.exe可以直接看symbol
t      : type symbol
x      : enum symbol
q      : quit
r      : show source file
etypes : show all type

## Document
代码文档化

[Clear, Functional C++ Documentation with Sphinx + Breathe + Doxygen + CMake](https://devblogs.microsoft.com/cppblog/clear-functional-c-documentation-with-sphinx-breathe-doxygen-cmake)

### GITBOOK

### GITHUB
Tianocore项目使用了github.io来做为文档展示，参考这个来构建github.io网页：[github.io](https://pages.github.com)

### CONFLUENCE
[CONFLUENCE](https://www.atlassian.com/software/confluence)

### MEDIAWIKI
[MEDIAWIKI](https://www.mediawiki.org)

### DOXYGEN

### PLANTUML

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

## Browser
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

## CI
持续开发(CI/CD)

[TeamCity](https://www.jetbrains.com/teamcity)
[TeamCity VS Jenkins：选择正确的CI / CD工具](https://cloud.tencent.com/developer/article/1664894)
[谁才是世界上最好的 CI/CD 工具？](https://zhuanlan.zhihu.com/p/67805669)
[Azure DevOps](https://azure.microsoft.com/en-us/products/devops)

## ANALYSIS
静态分析

### COVERITY

### KLOCKWORK

## TEST
单元测试：以数据为中心进行测试

[OpenCppCoverage](https://github.com/OpenCppCoverage/OpenCppCoverage)
[C++开源代码覆盖率工具OpenCppCoverage介绍(Windows)](https://www.cnblogs.com/coderzh/p/OpenCppCoverage.html)
[GCOV使用    ](https://blog.csdn.net/lishenglong666/article/details/8056777)
[gcov使用小节](https://blog.csdn.net/weixin_41910194/article/details/80759473)

### CMOCKA

## Tracker
缺陷管控

### BUGZILLA

## REMOTE
[win10 开启ssh server服务 远程登录](https://blog.csdn.net/weixin_43064185/article/details/90080815)

[Key-based authentication in OpenSSH for Windows](https://learn.microsoft.com/en-us/windows-server/administration/openssh/openssh_keymanagement): authorized_keys, administrators_authorized_keys
[Get started with OpenSSH for Windows           ](https://learn.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse)

[Linux系统SSH客户端断开后保持进程继续运行配置方法](https://help.aliyun.com/document_detail/42523.html)

[保持ssh session在断开连接后保持运行的五种方法](https://blog.csdn.net/qq_34769162/article/details/107948168)

[xvfb 初步探究](https://blog.csdn.net/span76/article/details/11473315)

https://www.openssh.com
https://www.realvnc.com

https://github.com/openssh/openssh-portable
https://github.com/PowerShell/openssh-portable

scp -P
ssh -p -l

[warning: agent returned different signature type ssh-rsa (expected rsa-sha2-512) when key registered with ssh-agent](https://github.com/PowerShell/Win32-OpenSSH/issues/1551): 使用ssh -V发现笔记本是8x的ssh没有这个问题，台式机是7x的有问题。这个问题导致了不能免密码登录。可以用git里面的ssh，试过没有问题。

### PUTTY
[PUTTY](https://putty.org)

## SEARCH
[BING SEARCH OPERATORS CHEAT SHEET: THE ULTIMATE GUIDE](https://www.sidegains.com/search-engines/bing-search-operators-cheat-sheet)
[搜网](http://sowang.com)

## NFC
https://blog.csdn.net/pingis58/article/details/125458697
https://blog.csdn.net/nfser_burn7/article/details/88565287
https://blog.csdn.net/zhang90283/article/details/108565846
https://nfctool.cn/4465/elementor-4465
https://bbs.pediy.com/thread-255182.htm
https://www.anquanke.com/post/id/254013


https://github.com/microsoft/mu_tiano_plus
https://github.com/microsoft/mu_basecore

https://www.busybox.net
git://busybox.net/busybox.git

[Logical Structure of a Hard Disk MBR DBR FAT and root](http://www.p-dd.com/chapter3-page18.html)

[Compiling and Installing Jansson](https://jansson.readthedocs.io/en/2.8/gettingstarted.html)
[window下jansson安装和使用](https://blog.csdn.net/zhangge3663/article/details/83617457)

[Big Endian and Little Endian](https://www.tutorialspoint.com/big-endian-and-little-endian)
Little Endian − In this scheme, low-order byte is stored on the starting address (A) and high-order byte is stored on the next address (A + 1).
Big Endian − In this scheme, high-order byte is stored on the starting address (A) and low-order byte is stored on the next address (A + 1).

[Elixir](https://elixir.bootlin.com/linux/latest/source)

[计算机程序](https://baike.baidu.com/item/程序/13831935)
[计算机软件](https://baike.baidu.com/item/软件/12053)
[指令      ](https://baike.baidu.com/item/指令/3225201)

https://github.com/google
https://github.com/oracle
https://github.com/oracle/opengrok
https://github.com/microsoft
https://github.com/intel
https://github.com/amd
https://github.com/ibm
https://github.com/samsung
https://github.com/apple
https://github.com/huawei
https://github.com/xiaomi
https://github.com/vivo
https://github.com/facebook
https://github.com/lenovo
https://github.com/alibaba
https://github.com/bytedance
https://github.com/baidu
https://github.com/yahoo

https://github.com/openssh
https://github.com/openssl
https://github.com/git
https://github.com/vim
https://github.com/universal-ctags

https://github.com/tianocore
https://github.com/qemu
https://github.com/llvm
https://github.com/powershell
https://github.com/python
https://github.com/wireshark

https://gitee.com/bytedance
https://gitee.com/baidu
