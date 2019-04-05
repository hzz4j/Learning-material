
> ubuntu 18.04LTS下常用的软件


## 网易云音乐

1. 配置命令行快捷键，以后在终端直接输入music启动

```
vi ~/.bashrc
进入编辑模式
alias music='sudo -b netease-cloud-music </dev/null &>/dev/null'
保存并退出
source ~/.bashrc
```

2. 点击图标，然后打开关机界面--[知乎: ubuntu下打开网易云](https://www.zhihu.com/question/277330447)

> 每次打不开的时候
我就右上角点击电源，佯装要poweroff
然后他就立马出来了
反正很玄学


## XX-Net


```
vi ~/.bashrc
cd到安装目录
alias xxnet='cd /home/hzz/Documents/XX-Net-3.13.1 && /bin/sh ./start'
```

> 目前是启动xxnet后不能关闭该终端


## sphinx

[安装参照博客](https://www.cnblogs.com/zhaojiedi1992/p/zhaojiedi_python_013_rst_spinx.html) 以及[官网](http://www.sphinx-doc.org/en/master/usage/quickstart.html)

> [更加详细的文档](https://docs.readthedocs.io/en/stable/intro/getting-started-with-sphinx.html#quick-start-video)


```
conda install sphinx
conda install -c conda-forge restructuredtext_lint 
```


### 主题

[主题官网](https://sphinx-themes.org/)

> 需要安装 **sphinx_theme** [官网](https://pypi.org/project/sphinx-theme/)

```bash
pip install sphinx_theme
```

选择一个主题，然后点击conf.py,复制相应的代码到自己的conf.py,如：

```python
#---sphinx-themes-----
html_theme = 'neo_rtd_theme'
import sphinx_theme
html_theme_path = [sphinx_theme.get_html_theme_path()]
```