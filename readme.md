# **py2msi**

## Introduction
本软件是一个可自动将python脚本文件打包成windows 下的可执行程序
(.exe)或安装程序(.msi)。

## Usage
1. File菜单：
Exit:退出程序。

2. Level菜单：

Basic:对打包的程序进行基本的设定，如指定脚本，打包后程序的名称，
版本号，程序描述等。

Deepin：对打包的程序进行深度定制，如指定程序的图标，所要排除的包，
所要排除的dll文件，所要包含的文件(readme.md,GUI界面图像等)。(本部分尚未实现)

3. Engine菜单:

cx_Freeze:基于cx_Freeze引擎打包。

py2exe:基于py2exe引擎打包。(本部分尚未实现)

pyinstaller:基于pyinstaller引擎打包。(本部分尚未实现)

4. install pkgs按钮:安装必要的第三方库。

generate exe按钮：生成windows下可执行文件(executable file)。
点击按钮，将会在脚本文件的同一文件夹下生成一个build文件夹，
可执行程序在build文件夹的子文件夹中。
以本程序为例，py2msi.py为本程序的脚本，位于F盘，点击按钮，
将会在F盘中生成build文件夹，而最终的目标程序路径为F:\build\exe.win32-2.7\py2msi.exe,如需发布程序，应该将该文件夹下其他文件一起发布，否则程序将不能正常运行。
（事实上，用目前版本的本软件生成的程序将会含有不少的冗余文件，如果你碰巧漏掉
或删除的文件不是你的程序运行所必需的，将不会造成影响。）

generate msi按钮：生成windows下的安装文件(Windows installer)。
点击按钮，将会在脚本文件的同一文件夹下生成一个build文件夹和一个dist文件夹。
build文件夹中的内容与点击generate exe 按钮生成的完全相同，而在dist文件夹中
将有一个msi文件，该msi文件即为目标文件，如需发布程序，直接将msi文件发布即可。

## Todo:
增加深度定制功能。

增加py2exe引擎。

增加pyinstaller引擎。

## Notice:
通过本程序生成的软件(无论是exe版本的还是msi版本的)不能确保你的源码不被反编译。

## Feedback:
有任何疑问或建议欢迎反馈。



