# **py2msi**

## Introduction
本软件是一个可自动将python脚本文件打包成windows 下的可执行程序
(.exe)或安装程序(.msi)。

## Usage
File菜单：
Exit:退出程序。

Level菜单：
Basic:对打包的程序进行基本的设定，如指定脚本，打包后程序的名称，
版本号，程序描述等。

Deepin：对打包的程序进行深度定制，如指定程序的图标，所要排除的包，
所要排除的dll文件，所要包含的文件(readme.md,GUI界面图像等)。(本部分尚未实现)

Engine菜单:
cx_Freeze:基于cx_Freeze引擎打包。
py2exe:基于py2exe引擎打包。(本部分尚未实现)
pyinstaller:基于pyinstaller引擎打包。(本部分尚未实现)

install pkgs按钮:安装必要的第三方库。
generate exe按钮：生成windows下可执行文件(executable file)。
generate msi按钮：生成windows下的安装文件(Windows installer)。

## Todo:
增加深度定制功能。
增加py2exe引擎。
增加pyinstaller引擎。

## Feedback:
有任何疑问或建议欢迎反馈。



