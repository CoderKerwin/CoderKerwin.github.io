# python
vendor: Python Software Foundation  
website: python.org  
support: windows/linux

Python is one of the most popular programming languages in use today. It has become the de-facto programming language for test automation, dev-ops, AI/ML and various other use cases

## install
linux: apt install python3, apt install python3-pip  
windows: download msi and double click msi

## run
linux: python3, python3 -m pip  
windows: py -3, py -3 -m pip

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
- subprocess
- threading
- json
- ctypes
 - int.from_bytes
 - int.from_buffer
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
- struct
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
 - open
 - exec
 - input
 - locals
 - vars
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
- dict()
- bytes()
 - copy_from_buffer
- bytearray()
 - byte_arrary()

- range()

- type()

- help()

- exit()
- quit()

- map()
 - list(map())

- filter()

### functions

- hex()
- len()
- vars()

- input()

- locals()

## packages

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

## practices

```
python -m pip install -i https://pypi.tuna.tsinghua.edu.cn/simple --upgrade pip
python -m pip install -i https://pypi.tuna.tsinghua.edu.cn/simple some-package

python -m pip config set global.extra-index-url "<url1> <url2>..."
python -m pip --proxy {proxy_server} install {module}
```

## refer

1. [os                          ](https://docs.python.org/3/library/os.html)
2. [XML Processing Modules      ](https://docs.python.org/3/library/xml.html)
3. [Minimal DOM implementation  ](https://docs.python.org/3/library/xml.dom.minidom.html#module-xml.dom.minidom)
4. [Dictionary Objects          ](https://docs.python.org/3/c-api/dict.html)
5. [文档对象模型API             ](https://docs.python.org/zh-cn/3/library/xml.dom.html)
6. [collections --- 容器数据类型](https://docs.python.org/zh-cn/3/library/collections.html#module-collections)
7. [urllib.request              ](https://docs.python.org/3.9/library/urllib.request.html#module-urllib.request)

8. [os.py        ](https://github.com/python/cpython/blob/3.10/Lib/os.py)
9. [posixmodule.c](https://github.com/python/cpython/blob/main/Modules/posixmodule.c)

10. [python解析XML            ](https://blog.csdn.net/qdPython/article/details/115520713)
11. [pythonos,Python os.fchdir](https://blog.csdn.net/weixin_28995873/article/details/11617561)

12. [python3正则表达式](https://www.runoob.com/Python3/python-reg-expressions.html)

13. [python文件操作](https://www.cnblogs.com/renpingsheng/p/8372083.html)

14. [python3 reload               ](https://blog.csdn.net/fly910905/article/details/74490784)
15. [Python3中matplotlib安装和使用](https://blog.csdn.net/beishanyingluo/article/details/103748934)

16. [matplotlib中plot.show()不显示图片的问题：如何把backend=Agg配置为TkAgg](https://blog.51cto.com/SpaceVision/3086976)

17. [解决No module named tkinter                       ](https://blog.csdn.net/qq_44685584/article/details/128600219)
18. [Python使用 turtle 模块报错 no module named tkinter](https://blog.csdn.net/u012308586/article/details/103061262)

19. [tkinter学习教程（一）](https://zhuanlan.zhihu.com/p/143478496)

20. [python pickle模块TypeError: write() argument must be str, not bytes](https://blog.csdn.net/lwgkzl/article/details/84764705)

21. [Matplotlib学习手册A006_Figure的add_subplot()方法](https://blog.csdn.net/sinat_32570141/article/details/103212790)

22. [difflib模块文件内容差异对比](https://www.cnblogs.com/Jabe/p/8948125.html)

23. [difflib — 字符比较](https://learnku.com/docs/pymotw/difflib-character-comparison)

24. [filecmp --- 文件及目录的比较](https://docs.python.org/zh-cn/3/library/filecmp.html)

25. [python写入html文件中文乱码-解决办法](https://blog.csdn.net/qq_40147863/article/details/81746445)

26. [在Python中创建、生成稀疏矩阵（均匀分布、高斯分布）](https://blog.csdn.net/weixin_46584887/article/details/123463305)

27. [XML处理模块                                  ](https://docs.python.org/zh-cn/3/library/xml.html)
28. [xml.dom --- 文档对象模型 API                 ](https://docs.python.org/zh-cn/3/library/xml.dom.html)
29. [xml.etree.ElementTree --- ElementTree XML API](https://docs.python.org/zh-cn/3/library/xml.etree.elementtree.html)

30. [Python map() 函数](https://www.runoob.com/python/python-func-map.html)

31. [Python实现Tab自动补全和历史命令管理的方法](https://www.ycpai.cn/python/Fv2T2Rgw.html)

32. [Windows下python的tab自动补全](https://www.cnblogs.com/51zf/p/9182791.html)

33. [Python 指定窗口截屏](https://www.cnblogs.com/guxingy/p/12201076.html)

34. [Python获取屏幕截图的4种方法](https://blog.csdn.net/jokerzhanglin/article/details/117201541)

35. [OpenCV+深度学习预训练模型，简单搞定图像识别教程](https://zhuanlan.zhihu.com/p/28703867)
36. [使用 OpenCV 对图像进行特征检测、描述和匹配     ](https://zhuanlan.zhihu.com/p/401188363)

37. [AttributeError: 'FigureCanvasTkAgg' object has no attribute 'show' and ValueError: Masked arrays must be 1-D](https://www.cnblogs.com/zhhy236400/p/9958889.html)

38. [Python frozenset() 函数的使用与作用](https://blog.csdn.net/weixin_48419914/article/details/121137418)

39. [教你如何利用python调用摄像头](https://blog.csdn.net/u014389734/article/details/109044080)

40. [基于python的音频处理--调用麦克风录音](https://blog.csdn.net/u014389734/article/details/109044080)

41. [最棒总结！Python日志库 logging 使用指南来了](https://zhuanlan.zhihu.com/p/445411809)

42. [PyGithub中获取私有仓库的pull_request的数据](https://blog.csdn.net/ls_python/article/details/119644558)

43. [Python3对字典操作时遇到错误：dictionary changed size during iteration](https://blog.csdn.net/zhihaoma/article/details/51265168)

44. [numpy.linalg.eig() 计算方形矩阵的特征值和特征向量](https://blog.csdn.net/strive_for_future/article/details/109631691)

45. [np.cov详解](https://blog.csdn.net/jeffery0207/article/details/83032325)

46. [Numpy中 cov() 的使用方法](https://blog.csdn.net/qq_41800366/article/details/88063772)

47. [细说Python的lambda函数用法](https://zhuanlan.zhihu.com/p/80960485)

48. [机器学习降维算法PCA](https://zhuanlan.zhihu.com/p/77151308)

49. [JSON](http://json.org/json-en.html)

50. [在 Python 中使用 requests 模块实现 Curl 命令](https://www.delftstack.com/zh/howto/python/implement-curl-commands-using-requests-module-in-python)

51. [pycurl-requests](https://pypi.org/project/pycurl-requests)

52. [Requests: HTTP for Humans](https://requests.readthedocs.io)

53. [PyPI 镜像使用帮助](https://mirrors.tuna.tsinghua.edu.cn/help/pypi)
54. [校园网联合镜像站](https://mirrors.cernet.edu.cn/list/pypi)
