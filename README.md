# jsForward-V2
解决web及移动端H5数据加密Burp调试问题


## 2022.6.2更新
> 对https://github.com/G-Security-Team/JS-Forward 做了二次修改，使用原生发包替代jquery，同时增加对https的支持，文件在Releases中。

> 使用方法类似，需要安装依赖：
```
pip install cryptography
pip install pyOpenSSL
pip install certifi
pip install urllib3==1.25.11
```

> python3脚本参数如下：
```
python Js-forward.py -t http -s xxx.example.com -i 192.168.101.33
-t 必须参数，指定http或者https
-s 必须参数，指定域名
-i 必须参数，指定burp监听地址
其中需要注意，Burp监听ip尽量别写127.0.0.1容易抓不到包,推荐写wifi对应ip
浏览器要先访问一次https://192.168.101.33/ 否则浏览器不会向该地址发包
```


> 关于工具的思路与原理请访问该项目查看：
```
https://github.com/G-Security-Team/JS-Forward
https://github.com/CTF-MissFeng/jsForward
```
