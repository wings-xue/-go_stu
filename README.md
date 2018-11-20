# -go_stu
学习go
最近迷上了docker和go。
还有大数据和分布式，看了spark，hadoop， yarn等一些东西。感觉写一个分布式的调度系统是一个很有意思的事情。

之前一直用python， 但是总感觉， 到了大型项目有心无力。

后面想做的很有意思阿。 学习下go开始写起来


### go get 添加代理
export http_proxy=http://127.0.0.1:1080
go get golang.org/xxx


### 另一种方法
mkdir -p $GOPATH/src/golang.org/x
cd $GOPATH/src/golang.org/x
git clone https://github.com/golang/net.git


```
# polipo配置
# This file only needs to list configuration variables that deviate
# from the default values.  See /usr/share/doc/polipo/examples/config.sample
# and "polipo -v" for variables you can tweak and further information.

logSyslog = true
logFile = /var/log/polipo/polipo.log

proxyAddress = "0.0.0.0"  
  
socksParentProxy = "127.0.0.1:1080"  
socksProxyType = socks5  
  
chunkHighMark = 50331648  
objectHighMark = 16384  
  
serverMaxSlots = 64  
serverSlots = 16  
serverSlots1 = 32  
# 重启polipo
/etc/init.d/polipo restart
# 设置代理
启动cow
cow 文档
https://github.com/cyfdecyf/cow
设置curl代理
export http_proxy=http://127.0.0.1:7777
export https_proxy=http://127.0.0.1:7777

"go.delveConfig": {
  "useApiV1": false,
  "dlvLoadConfig": {
    "followPointers": true,
    "maxVariableRecurse": 3,
    "maxStringLen": 400,
    "maxArrayValues": 400,
    "maxStructFields": -1
  }
}

https://itnext.io/golang-bits-better-debugging-in-vscode-599bc5b018da
vscode debug config
```
