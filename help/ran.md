#1 使用 Ran 做网页服务器

如果觉得安装 Python 有点儿麻烦，或者 Python 安装后双击 server.cmd 无法正常启动网页服务器，那么，可以用这个 Ran ，它的中文名叫做“燃”：

![Ran Logo](/assets/Ran.gif)

#2 下载
- 这个 Ran 很简单，就是一个 exe 文件，我放在这个网站了，点击下载即可：
[ran.0.1.4.zip](https://kepan.org/docsify/down/ran.0.1.4.zip)

#2 使用
- 下载后解压缩，里面只有两个文件：
> ran.exe
> server.cmd

- 把这两个文件，复制到你的 kepan-docsify 根目录下，覆盖原先的 `server.cmd` 即可。

- 双击 `server.cmd` ，就可以启动 Ran 作为网页服务器了。

- 如果这时有防火墙的提示窗口，点击允许访问即可。
![Firewall](/assets/Firewall.jpg)

- 然后打开浏览器，访问 `http://localhost/` 就能看到这个本地网站了。

#2 说明
`server.cmd` 里面只有一行命令：
 ```
 ran -p 80
 ```

 不用 `server.cmd` ，直接双击运行 `ran.exe` 其实也可以，但这时网页服务器的默认端口是 `8080` ，这时你需要通过 `http://localhost:8080/` 才能访问本地网站。

 用 `server.cmd` 来启动服务器的话，它使用的是默认的 `80` 端口，这时候直接使用 `http://localhost/` 就可以访问了。


#2 鸣谢

# Ran （燃）
这是一个用 Go 语言编写的简单网页服务器，这是一个开源项目：
    * https://github.com/m3ng9i/ran

