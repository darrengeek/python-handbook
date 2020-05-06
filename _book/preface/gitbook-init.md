# 全局安装 gitbook-cli
```
建议使用 npm 淘宝源：

npm config set registry https://registry.npm.taobao.org/

然后安装gitbook -cli

npm i -g gitbook-cli
```
第三部 初始化电子书
```
# 创建一个目录，进入
mkdir gitbook-demo
cd gitbook-demo
 
# 初始化电子书目录
gitbook init 
 
# 编译电子书
gitbook serve 
```

#### 说明一下：
init 以后，目录里会有这两个文件 README.md 和 SUMMARY.md，README.md 是对电子书的简单介绍，SUMMARY.md 是电子书的目录结构。

# 目录结构长这样：
* [电子书名称](README.md)
* [第一章](chapter1/README.md)
    * [xxxx](chapter1/section1.1.md)
    * [xxxx](chapter1/section1.2.md)
* [第二章](chapter2/README.md)
    * [xxxx](chapter2/section2.1.md)
    * [xxxx](chapter2/section2.2.md)

编写 SUMMARY.md，执行 gitbook init 生成目录结构文件，然后编写各个文件夹中生成的文件。

最后 gitbook serve。

gitbook serve 命令实际上会首先调用 gitbook build 编译书籍，完成以后会打开一个 web 服务器，监听在本地的 4000 端口

# 参考链接
1.https://www.cnblogs.com/liyao0312/p/11334655.html
2.