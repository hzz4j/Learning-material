
## 从分支中拿文件

[How to get just one file from another branch](https://stackoverflow.com/questions/2364147/how-to-get-just-one-file-from-another-branch)

> 从分支中取一个文件到master,并不是合并

```bash
git checkout master               # first get back to master
git checkout experiment -- app.js # then copy the version of app.js 
                                  # from branch "experiment"
```