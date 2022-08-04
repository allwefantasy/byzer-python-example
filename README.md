## Byzer-python

本项目主要演示 Byzer-python 的使用。

## 安装 Byzer 桌面版

安装 Visual Studio Code。 [下载地址](https://code.visualstudio.com/) 然后安装他。

> 注意： 请使用 [Light Color Theme](https://code.visualstudio.com/docs/getstarted/themes) 以获得更好的用户体验

![](https://github.com/allwefantasy/byzer-visualization-example/example-data/v2-cb68ef1b333871371228bd23fa704dac_720w.jpg)


接着你可以根据操作系统，下载合适的 Byzer 扩展：

1. [Mac](https://download.byzer.org/byzer/2.3.2/byzer-vscode-extension-darwin-0.0.7.vsix)
2. [Linux](https://download.byzer.org/byzer/2.3.2/byzer-vscode-extension-linux-0.0.7.vsix)
3. [Windows](https://download.byzer.org/byzer/2.3.2/byzer-vscode-extension-win-0.0.7.vsix)


> Warnning: Windows 暂时不支持 Byzer-python,所以无法使用该项目。

点击 Visual Studio Code 中的 扩展(Extensions) 或者 View: Extensions command (Ctrl+Shift+X)

![](https://github.com/allwefantasy/byzer-visualization-example/example-data/v2-c801c3123d1427d35661851eeec15f5c_720w.jpg)

选择已经下载的好的 VSIX 文件 然后安装。

## Python 环境

Byzer-python 依赖于 Python, 用户需要在本机安装 [Miniconda](https://docs.conda.io/en/latest/miniconda.html)。
接着在本项目中执行如下指令：

```
conda env create --file environment.yml
```

这样可以得到一个名字叫做 `ray-1.12.0` 的环境。

## 运行时配置

根目录下的 `.mlsql.config` 可以配置包括 JDK 以及 Byzer 的一些运行时参数诸如内存大小。 
如果你出现类似 `chmod` 找不到等问题，那么可以设置下JDK。比如：

```
java.home=/Library/Java/JavaVirtualMachines/jdk1.8.0_151.jdk/Contents/Home/
engine.memory=6048m

user.owner=admin
user.access_token=123
user.outputSize=100
```