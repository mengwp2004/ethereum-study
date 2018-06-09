##运行eth test,very important


https://github.com/ethereum/go-ethereum/wiki/Developers'-Guide

#1 Go Environment

We assume that you have go v1.8 installed, and GOPATH is set.

Note:You must have your working copy under $GOPATH/src/github.com/ethereum/go-ethereum

git clone git@github.com:nirname/go-ethereum.git $GOPATH/src/github.com/ethereum/go-ethereum

#2 Managing Vendored Dependencies

All other dependencies are tracked in the vendor/ directory. We use govendor to manage them.

If you want to add a new dependency, run govendor fetch <import-path>, then commit the result.

#3 Building Executables

Switch to the go-ethereum repository root directory.

You can build all code using the go tool, placing the resulting binary in $GOPATH/bin

go install -v ./cmd/geth

#4 Testing

Testing one library:

go test -v -cpu 4 ./eth  

go test -v -cpu 4 ./eth -run TestMethod

bluesky@bluesky-ThinkPad-T430:/mwp/work/study/economy/go-work/src/github.com/ethereum/go-ethereum$ go test -v -cpu 4 ./crypto -run TestKeccak256Hash
=== RUN   TestKeccak256Hash
--- PASS: TestKeccak256Hash (0.00s)
PASS
ok  	github.com/ethereum/go-ethereum/crypto	0.027s

 

go test -v -cpu 4 ./eth -run TestRecvTransactions62
=== RUN   TestRecvTransactions62
--- PASS: TestRecvTransactions62 (0.00s)
PASS
ok  	github.com/ethereum/go-ethereum/eth	0.047s



#ethereum 参考文档

https://ethereum.gitbooks.io/frontier-guide/content

#交易所
www.btcbl.com
https://btcbl.com/index.php?s=/User/Secure/secure

#下载公链数据
geth --fast --cache=1024 console

#使用公有钱包
在money-tools目录下，运行./ethereumwallet

install dlv 程序，方便调试
https://github.com/derekparker/delve/blob/master/Documentation/cli/getting_started.md

调试go程序
dlv debug max.go

gdb调试
 go build -gcflags "-N -l"  max.go 


包括mist在私链上的应用

http://blog.csdn.net/vinsuan1993/article/details/77144263

http://blog.csdn.net/xiabing082/article/details/77368624

如何启动mist
https://blog.csdn.net/ziyuzhiye/article/details/54291744

geth结构分析

http://blog.csdn.net/xiabing082/article/details/77368624
