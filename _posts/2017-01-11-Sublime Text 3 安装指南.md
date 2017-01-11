---
layout: post
title:  "Sublime Text 3 安装指南"
key: 10001
tags: blog

date: 2017-01-11 16:59:00
---

# Sublime Text 3 安装指南

------

### 1.下载安装Sublime
[http://www.sublimetext.com/3](http://www.sublimetext.com/3)

### 2.安装Package Control组件

按Ctrl+`调出console（注意与其他软件快捷键的冲突）

粘贴以下代码到底部命令行并回车：

```
import urllib.request,os; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); open(os.path.join(ipp, pf), 'wb').write(urllib.request.urlopen( 'http://sublime.wbond.net/' + pf.replace(' ','%20')).read())
```

重启Sublime Text 3。
如果在Perferences->package settings中看到package control这一项，则安装成功。
