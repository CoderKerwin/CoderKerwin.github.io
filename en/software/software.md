# software

## EDITOR

### VIM

https://www.vim.org, https://github.com/vim

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

Zi, /debug

#### GCC

-g

#### CLANG

## JAVA COMPILER

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

http://www.doxygen.nl/download.html

### PLANTUML

### READTHEDOC

https://about.readthedocs.com

### SPHINX

https://www.sphinx-doc.org

[Clear, Functional C++ Documentation with Sphinx + Breathe + Doxygen + CMake](https://devblogs.microsoft.com/cppblog/clear-functional-c-documentation-with-sphinx-breathe-doxygen-cmake)

[Sphinx + Read the Docs 从懵逼到入门](https://zhuanlan.zhihu.com/p/264647009)

### GITBOOK

### GITHUB
Tianocore项目使用了github.io来做为文档展示，参考这个来构建github.io网页：[github.io](https://pages.github.com)

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

