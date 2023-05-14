# python
vendor: Python Software Foundation
website: python.org
support: windows/linux

Python is one of the most popular programming languages in use today. It has become the de-facto programming language for test automation, dev-ops, AI/ML and various other use cases

## install
linux: apt install python3, apt install python3-pip
windows: download msi and double click msi

## run
linux: python3 <python script>, python3 -m pip
windows: py -3 <python script>, py -3 -m pip

## data type
- str()
- int()
- float()
- list()
- dict()
- bytes()
- bytearray()

## modules

- os
 - os.path
 - os.sep
 - os.popen
 - os.system
 - os.unlink
 - os.symlink
 - os.getcwd()
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
- importlib
 - importlib.reload

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

### modules

- sys
 - sys.path  : Search module from this path, can append path to make module can be searched
 - sys.stdin
 - sys.stdout

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
random.rand(4,4): generate random 4x4 array
randMat = mat(random.rand(4,4)): Change array to matrix
randMat.I: Inverse matrix
randMat * randMat.I = Identity matrix
eye(4): Create 4x4 Identity matrix

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

16. [PyPI 镜像使用帮助](https://mirrors.tuna.tsinghua.edu.cn/help/pypi)
17. [校园网联合镜像站](https://mirrors.cernet.edu.cn/list/pypi)
