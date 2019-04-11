
[linuxsurvival](https://linuxsurvival.com/linux-tutorial-module-3-introduction/)

## Module 3

### man

manual 

> man man 

try to find what you want 

> man -k keyword 

**you can ignore any commands which have a section other than '1'.**



### finger

The finger displays information about the system users.


### find

search for files in a directory hierarchy

> find startplace -name filename

> find ~ -name "毕业设计*"



### cat

concatenate(串联)

combined files and default will send its output to your screen

> cat joke-1 joke-2

![](./imgs/cat.png)




一般会有人使用cat来查看文件内容，但是还是建议使用more来查看

send the output from a command such as "cat" to a file, you can use either '>' or '>>'.

('>' overwrite),('>>' append),**arrow pointing to where you want the output to go.** **redirecting output**

![](./imgs/cat-2.png)


### line print

#### lpr

将文本发送到打印设备
> lpr -P zephyr corny
![](./imgs/cat-3.png)


### lpq

line printer queue

check on the status of your print job

![](./imgs/cat-4.png)



### lprm

line printer remove

cancel your print job

![](./imgs/cat-5.png)


## Module 4


### cp,rm

The regular "cp" command will not let you copy directories, but if you use the "-r" option, it will. 



 "rmdir" command only deletes empty.

### 磁盘文与文件系统


#### df

> disk free： disk usage list

Notice that the "Used" and "Available" columns do not add up to the "1k-blocks" (total) column. That is because a percentage of the disk is always set aside for administrative use.


> The "Mounted on" column shows where the disks reside in your filesystem tree.

![](./imgs/file.png)



#### 硬盘挂载在文件系统

Each (hard drive)(硬盘) is "mounted" on a particular directory in that tree. 

For example, the first hard drive is mounted on "/", the root of the tree. Everything contained on that drive has been colored yellow in the diagram at bottom right. The second drive is mounted on "/home". That means that any files or directories under "/home" in the tree will be stored on the second drive rather than on the first one. They are colored blue. Similarly, the third drive has been mounted on "/usr". Its contents have been colored green.

![](./imgs/file-1.png)



------------

figure out which disk contains a particular file or directory and then display statistics **only for that disk**.

>  find out how much disk space is free on the disk where your current directory resides

> df .
