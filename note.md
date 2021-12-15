# Lecture 1
## note index
* Linux是怎么解析一段命令（command）的？如果想要在参数（argument）中出现空格怎么办？ 
* shell是怎么找到命令程序（program）的？
* ls -l 前面的一系列字母什么意思？配合食用：[here](https://www.computerhope.com/unix/uchmod.htm)
* shell中```>```,```<```,```<<```,```|```的用法

add：
* 在两个路径之间反复横跳：```cd -```
```cd -```回到上一次所在的路径
## exercise:
* 为什么```sh semester```可以运行而```./semester```不能运行？
```sh filename```是启动bash interpreter，把文件作为参数传进去，所以```sh semester```与```echo Hello```本质上没有什么区别
```./semester```不能运行应该是因为权限问题，使用```chmod```命令修改权限就能运行了
* 通过```./semester```运行时，shell是怎么知道运行```sh```?
>if a script is named with the path path/to/script, and it starts with the following line, #!/bin/sh, then the program loader is instructed to run the program /bin/sh, passing path/to/script as the first argument. -Wikipedia

more details：see [shebang](https://en.wikipedia.org/wiki/Shebang_(Unix))


## other resources:
 * Linux chmod command：[here](https://www.computerhope.com/unix/uchmod.htm)
