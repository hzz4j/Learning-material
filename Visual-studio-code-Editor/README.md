## Java输入问题

> 会在该IDE中打开一个输入窗口,重点是更改console: integratedTerminal

**launch.json 这个文件在.vscode目录下**
```java
{
    "configurations": [
        {
            "type": "java",
            "name": "CodeLens (Launch) - Main",
            "request": "launch",
            "mainClass": "Main",
            "console": "integratedTerminal"
        },
        {
            "type": "java",
            "name": "CodeLens (Launch) - Solution",
            "request": "launch",
            "mainClass": "Solution",
            "console": "integratedTerminal"
        }
    ]
}
```




调试的时候直接点击debug

![](./imgs/1.PNG)




## vscode 使用cmder作为终端

更改settings

1. 注释原来的cmd.exe
2. 添加新的配置，路径为自己的cmder安装位置

```json
    // "terminal.integrated.shell.windows": "C:\\windows\\System32\\cmd.exe",
    "terminal.integrated.shell.windows": "cmd.exe",
    "terminal.integrated.env.windows": {
    "CMDER_ROOT": "C:\\tools\\cmder"
    },
```







## 快速运行一个Java脚本

[Visual Studio Code for Java: the Ultimate Guide 2019](https://dzone.com/articles/visual-studio-code-for-java-the-ultimate-guide-201)

![](./imgs/2.PNG)





## Override方法


![](https://user-images.githubusercontent.com/148698/28883373-29ed282a-777c-11e7-9035-700718d549b1.gif)


## vscode插件

### setter & getter方法

+ 插件  [Java Code Generators](https://marketplace.visualstudio.com/items?itemName=sohibe.java-generate-setters-getters)


### Prettier - Code formatter

> 保存自动格式美化代码

settings设置editor.formatOnSave 为true,即勾选


### 导入jar包

> 创建lib文件夹，将jar包放到里面

1. 最好的方式的用eclipse打开项目，使用java build path 添加jar包,将依赖的jar包写入.classpath文件中。这样方法适合很多jar包一次性配置。
2. 也可以手动添加 在.classpath文件中添加
```
<classpathentry kind="lib" path="lib/spring-aop-5.1.7.RELEASE-sources.jar"/>
```



## 快捷键

1. ctrl+enter 下一行
2. ctrl+` 打开终端
3. ctrl+shift+a 快速注释代码块
4. ctrl+end  快速到文件末尾
