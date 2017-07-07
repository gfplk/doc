# ubuntu修改软件源

* ubuntu默认配置在/etc/apt/sources.list
        可以直接将要修改的配置放到这个文件里

        apt update
        就可以了。

* 还有另外一种办法:
        /etc/apt/sources.list.d/
        直接将其它的源放到这里文件中以.list结尾
        apt update就ok了。


* 附上ustc中国科学技术大学的软件源
```
http://mirrors.ustc.edu.cn/help/ubuntu.html
```
