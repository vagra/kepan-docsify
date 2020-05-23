#1 使用 Python 做网页服务器


通过一行简单的命令就可以使用 Python 的网页服务器：
```
python -m http.server 80
```

但这样就需要先安装 Python ：

- 下载地址： https://www.python.org/downloads/windows/

- 下载最新版的 `Windows x86-64 executable installer` 即可；

- 安装时一定要勾选下面的 `Add Python 3.x to PATH` 选项：
![Install Python](/assets/Install_Python.jpg)

装好 Python 以后，直接双击执行 kepan-docsify 目录下的 server.cmd ， Python 的网页服务器就启动了。

然后用浏览器访问 `http://localhost/` ，就可以看到这个本地网站了。