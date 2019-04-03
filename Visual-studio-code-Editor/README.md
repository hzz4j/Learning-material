## Java输入问题

> 会在该IDE中打开一个输入窗口

**launch.json**
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