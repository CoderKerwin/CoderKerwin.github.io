# python
vendor: Python Software Foundation  
website: <https://www.python.org>  
docs: <https://docs.python.org>  
repos: <https://pypi.org>  
support: windows/linux  
uefi-python: <https://github.com/tianocore/edk2-libc/tree/master/AppPkg/Applications/Python/Python-3.6.8>

Python is one of the most popular programming languages in use today. It has become the de-facto programming language for test automation, dev-ops, AI/ML and various other use cases

## install
linux: `apt install python3`, `apt install python3-pip`  
windows: install from msi

## run
linux: `python3`, `python3 -m pip`  
windows: `py -3`, `py -3 -m pip`

## data type

int,
float,
str,
tuple,
list,
dict,
set,
bytes,
bytearray

## modules

- os
 - os.path
 - os.sep
 - os.popen
 - os.system
 - os.unlink
 - os.symlink
 - os.getcwd()
- sys
 - sys.path  : Search module from this path, can append path to make module can be searched
 - sys.stdin
 - sys.stdout
- platform
- time
- re
 - re.compile
 - re.findall
 - re.match
- hashlib
- socket
- ipaddress
- argparse
 - argparse.ArgumentParser
 - argparse.add_argument
 - argparse.FileType
- shutil
 - shutil.copy
- json
- pathlib
- importlib
 - importlib.import_module
 - importlib.metadata
  - distribution(dist_name).entry_points
 - importlib.reload
- urllib
 - urllib.request
  - urllib.request.urlopen
  - urllib.request.build_opener
  - urllib.request.Request
- uuid
- turtle
- tkinter
- math
- random
- traceback
 - traceback.print_exc
- binascii
- filecmp
- difflib

## builtins

- builtins
 - globals
  - globals().setdefault('load_entry_point', importlib_load_entry_point)
 - next
  - next(matches).load()

### classes

- str()
 - copy
- int()
- float()
- list()
 - index() for example `print('percent %d'.format(list).index(item)/len(list))` pay attention that it only show **first matched item** so make sure that there are **no same item** in list
- dict()
 - items() will return tuple. you can not use dict() as list directly because it just mean keys(). can use list(dict()) and list(dict().items()) to know the difference
- bytes()
 - copy_from_buffer
- bytearray()
 - byte_arrary()

- exit()
- quit()

- filter()

## Packages

SSHv2: https://www.paramiko.org
```
ssh = paramiko.SSHClient()  # Create SSH object
ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())  # allow connect to the host that not exist in know_hosts file
ssh.connect(args.address, 22, user, password)  # connect server
stdin, stdout, stderr = ssh.exec_command('ls')
cmd='journalctl --since=\"{}\"'.format('May 14 2023')
stdin, stdout, stderr = ssh.exec_command(cmd)
ssh.close()  # Close connection
```

HTTP: https://requests.readthedocs.io
```
from requests.packages.urllib3.exceptions import InsecureRequestWarning
requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
resp = requests.post('https://{}'.format(args.address), data=file.read(), verify=False, auth=(args.username, args.password))
```

Name:    numpy  
Website: https://www.numpy.org
```
random.rand(4,4): generate random 4x4 array
random.shuffle(arr): random the array
randMat = mat(random.rand(4,4)): Change array to matrix
randMat.I: Inverse matrix
randMat * randMat.I = Identity matrix
eye(4): Create 4x4 Identity matrix
mean: arithmetic mean
var: variance
nonzeros: return (array(a), array(b)) for example, nonzeros([[1,0],[0,1]]) will return (array(0,1), array(0,1)) which mean 0x0 and 1x1 is nonzero
```

Name:    scipy  
Website: https://www.scipy.org

Name:    paramiko  
Website: https://www.paramiko.org 

Name:    matplotlib  
Website: https://matplotlib.org

## Practices

```
python -m pip install -i https://pypi.tuna.tsinghua.edu.cn/simple --upgrade pip
python -m pip install -i https://pypi.tuna.tsinghua.edu.cn/simple some-package

python -m pip config set global.extra-index-url "<url1> <url2>..."
python -m pip --proxy {proxy_server} install {module}
```

``os.path.sep.join('/'.join(r'\a/b/c\d\e\f'.split(r'\')).split('/'))``可用于将windows与linux混合路径转化为系统特定路径  
``r'\a/b/c\d\e\f'.split(r'\')``转换字符串为列表['','a/b/c','d','e','f']  
``'/'.join(r'\a/b/c\d\e\f'.split(r'\'))``转换列表为字符串'/a/b/c/d/e/f'  
``'/'.join(r'\a/b/c\d\e\f'.split(r'\')).split('/')``再次转换字符串为列表['','a','b','c','d','e','f']  
``'->'.join('/'.join(r'\a/b/c\d\e\f'.split(r'\')).split('/'))``转换字符串为'->a->b->c->d->e->f'  
``os.path.sep``是特定系统的分隔符  
os.path里面是否已经存在自动转换路径的函数？可否将这个方法加到os.path里面？

## References

### Mirror
1. [PyPI镜像使用帮助](https://mirrors.tuna.tsinghua.edu.cn/help/pypi)
2. [校园网联合镜像站](https://mirrors.cernet.edu.cn/list/pypi)

### Official Python Documentation
1.  <https://docs.python.org/3/tutorial/errors.html>
2.  <https://docs.python.org/3/reference/datamodel.html>
3.  <https://docs.python.org/3/c-api/dict.html>
4.  <https://docs.python.org/3/library/functions.html>: range(), map(), reversed(), set(), enumerate(), all(), any(), sum(), super(), vars(), zip(), input(), iter(), next(), chr(), ord(), locals(), hex(), len(), help(), type(), open(), exec(), globals(), format(), sorted(), etc
5.  <https://docs.python.org/3/library/unittest.html>
6.  <https://docs.python.org/3/library/os.html>
7.  <https://docs.python.org/3/library/netrc.html>
8.  <https://docs.python.org/3/library/getpass.html>
9.  <https://docs.python.org/3/library/urllib.html>
10. <https://docs.python.org/3/library/itertools.html>
11. <https://docs.python.org/3/library/sched.html>
12. <https://docs.python.org/3/library/timeit.html>
13. <https://docs.python.org/3/library/asyncio.html>
14. <https://docs.python.org/3/library/email.html>
15. <https://docs.python.org/3/library/xml.html>
16. <https://docs.python.org/3/library/filecmp.html>
17. <https://docs.python.org/3/library/collections.html>
18. <https://docs.python.org/3/library/pickle.html>
19. <https://docs.python.org/3/library/html.html>
20. <https://docs.python.org/3/library/string.html>: asciis string constants and format string syntax
21. <https://docs.python.org/3/library/stdtypes.html>: str.format(), bytes.decode(), dict.update()
22. <https://docs.python.org/3/library/ctypes.html>: from_buffer
23. <https://docs.python.org/3/library/struct.html>: pack
24. <https://docs.python.org/3/library/subprocess.html>: run()
25. <https://docs.python.org/3/library/threading.html>
26. <https://docs.python.org/3/library/csv.html>: fileld_size_limit(), DictWriter()

### Github Python Repository
1. <https://github.com/python/cpython/blob/main/Lib/os.py>
2. <https://github.com/python/cpython/blob/main/Modules/posixmodule.c>

### Python Package Index

#### Visualization
1. <https://pypi.org/project/matplotlib>, <https://github.com/matplotlib/matplotlib>, <https://matplotlib.org/stable/users>

#### Data Science
1. <https://pypi.org/project/pandas>, <https://github.com/pandas-dev/pandas>, <https://pandas.pydata.org/docs/user_guide>
2. <https://pypi.org/project/numpy>,  <https://github.com/numpy/numpy>
3. <https://pypi.org/project/scipy>,  <https://github.com/scipy/scipy>

#### Machine Learning
1. <https://pypi.org/project/datasets>
2. <https://pypi.org/project/transformers>, <https://github.com/huggingface/transformers>
3. <https://pypi.org/project/torch>,        <https://github.com/pytorch/pytorch>
4. <https://pypi.org/project/tensorflow>,   <https://github.com/tensorflow/tensorflow>
5. <https://pypi.org/project/chatbotAI>

#### Graph Theory
1. <https://pypi.org/project/networkx>, <https://github.com/networkx/networkx>: all_simple_paths()

#### Network
1. <https://pypi.org/project/requests>: <https://github.com/psf/requests>
2. <https://pypi.org/project/pycurl-requests>

#### Security
1. <https://pypi.org/project/keyring>
2. <https://pypi.org/project/keyrings.cryptfile>: Need call `keyring.set_keyring(CryptFileKeyring())` to set this as backend
3. <https://pypi.org/project/credentials>
4. <https://pypi.org/project/cryptography>

#### Miscellanous
1. <https://pypi.org/project/Office365-REST-Python-Client>: <https://github.com/vgrem/Office365-REST-Python-Client>

### RUNOOB
1. [Python format 格式化函数](https://www.runoob.com/python/att-string-format.html)
2. [python3正则表达式       ](https://www.runoob.com/Python3/python-reg-expressions.html)
3. [Python map() 函数       ](https://www.runoob.com/python/python-func-map.html)

### CSDN
1.  [python解析XML                                                        ](https://blog.csdn.net/qdPython/article/details/115520713)
2.  [pythonos,Python os.fchdir                                            ](https://blog.csdn.net/weixin_28995873/article/details/11617561)
3.  [python3 reload                                                       ](https://blog.csdn.net/fly910905/article/details/74490784)
4.  [Python3中matplotlib安装和使用                                        ](https://blog.csdn.net/beishanyingluo/article/details/103748934)
5.  [解决No module named tkinter                                          ](https://blog.csdn.net/qq_44685584/article/details/128600219)
6.  [Python使用 turtle 模块报错 no module named tkinter                   ](https://blog.csdn.net/u012308586/article/details/103061262)
7.  [python pickle模块TypeError: write() argument must be str, not bytes  ](https://blog.csdn.net/lwgkzl/article/details/84764705)
8.  [Matplotlib学习手册A006_Figure的add_subplot()方法                     ](https://blog.csdn.net/sinat_32570141/article/details/103212790)
9.  [python写入html文件中文乱码-解决办法                                  ](https://blog.csdn.net/qq_40147863/article/details/81746445)
10. [在Python中创建、生成稀疏矩阵（均匀分布、高斯分布）                   ](https://blog.csdn.net/weixin_46584887/article/details/123463305)
11. [Python获取屏幕截图的4种方法                                          ](https://blog.csdn.net/jokerzhanglin/article/details/117201541)
12. [Python frozenset() 函数的使用与作用                                  ](https://blog.csdn.net/weixin_48419914/article/details/121137418)
13. [教你如何利用python调用摄像头                                         ](https://blog.csdn.net/u014389734/article/details/109044080)
14. [基于python的音频处理--调用麦克风录音                                 ](https://blog.csdn.net/u014389734/article/details/109044080)
15. [PyGithub中获取私有仓库的pull_request的数据                           ](https://blog.csdn.net/ls_python/article/details/119644558)
16. [Python3对字典操作时遇到错误：dictionary changed size during iteration](https://blog.csdn.net/zhihaoma/article/details/51265168)
17. [numpy.linalg.eig() 计算方形矩阵的特征值和特征向量                    ](https://blog.csdn.net/strive_for_future/article/details/109631691)
18. [np.cov详解                                                           ](https://blog.csdn.net/jeffery0207/article/details/83032325)
19. [Numpy中 cov() 的使用方法                                             ](https://blog.csdn.net/qq_41800366/article/details/88063772)
20. ['MRmean' object has no attribute 'mr'                                ](https://blog.csdn.net/wqqGo/article/details/80452294)
21. [python使用代理的几种方式                                             ](https://blog.csdn.net/whatday/article/details/112169945)
22. [如何使用python发送一条短信                                           ](https://blog.csdn.net/qq_41501331/article/details/106365515)
23. [python 发送邮件/正文插入表格                                         ](https://blog.csdn.net/qq_34864753/article/details/120769126)
24. [使用Python与Sharepoint进行交互                                       ](https://blog.csdn.net/mzl87/article/details/107325321): <https://shareplum.readthedocs.io/en/latest>

### ZHIHU
1. [tkinter学习教程（一）                          ](https://zhuanlan.zhihu.com/p/143478496)
2. [OpenCV+深度学习预训练模型，简单搞定图像识别教程](https://zhuanlan.zhihu.com/p/28703867)
3. [使用 OpenCV 对图像进行特征检测、描述和匹配     ](https://zhuanlan.zhihu.com/p/401188363)
4. [最棒总结！Python日志库 logging 使用指南来了    ](https://zhuanlan.zhihu.com/p/445411809)
5. [细说Python的lambda函数用法                     ](https://zhuanlan.zhihu.com/p/80960485)
6. [机器学习降维算法PCA                            ](https://zhuanlan.zhihu.com/p/77151308)
7. [如何理解Python中的yield用法?                   ](https://zhuanlan.zhihu.com/p/268605982)
8. [Python 定时任务最佳实践                        ](https://zhuanlan.zhihu.com/p/92152648): <https://github.com/dbader/schedule>
9. [5种基于Python文字转化语音方法                  ](https://zhuanlan.zhihu.com/p/439918609)

### CNBLOGS
1. [python文件操作                                                                                              ](https://www.cnblogs.com/renpingsheng/p/8372083.html)
2. [difflib模块文件内容差异对比                                                                                 ](https://www.cnblogs.com/Jabe/p/8948125.html)
3. [Windows下python的tab自动补全                                                                                ](https://www.cnblogs.com/51zf/p/9182791.html)
4. [Python 指定窗口截屏                                                                                         ](https://www.cnblogs.com/guxingy/p/12201076.html)
5. [AttributeError: 'FigureCanvasTkAgg' object has no attribute 'show' and ValueError: Masked arrays must be 1-D](https://www.cnblogs.com/zhhy236400/p/9958889.html)

### Miscellaneous
1. [用python发送表格数据到邮箱](https://www.jianshu.com/p/a04eafcc2f69)

2. [matplotlib中plot.show()不显示图片的问题：如何把backend=Agg配置为TkAgg](https://blog.51cto.com/SpaceVision/3086976)

3. [difflib — 字符比较](https://learnku.com/docs/pymotw/difflib-character-comparison)

4. [Python实现Tab自动补全和历史命令管理的方法](https://www.ycpai.cn/python/Fv2T2Rgw.html)

5. [JSON](http://json.org/json-en.html)

6. [在 Python 中使用 requests 模块实现 Curl 命令](https://www.delftstack.com/zh/howto/python/implement-curl-commands-using-requests-module-in-python)

7. [getpass() and getuser() in Python](https://www.geeksforgeeks.org/getpass-and-getuser-in-python-password-without-echo)

8. [Secure Password or Token on Windows – Python](https://techwizard.cloud/2022/02/09/secure-password-or-token-on-windows-python)

9. [Python SMTP.starttls方法代码示例](https://vimsky.com/examples/detail/python-ex-smtplib-SMTP-starttls-method.html)

10. [How to fix certificate verify failed](https://community.ibm.com/community/user/ibmz-and-linuxone/blogs/sheng-jie-han/2021/06/03/how-to-fix-certificate-verify-failed-self-signed-c)

11. [Command-line options](https://mrjob.readthedocs.io/en/latest/job.html)

12. [Working with Excel Files in Python](https://www.python-excel.org): [openpyxl](https://openpyxl.readthedocs.io/en/stable/tutorial.html)
