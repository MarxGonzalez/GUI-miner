你好！
很冒昧用这样的方式来和你沟通，如有打扰请忽略我的提交哈。我是光年实验室（gnlab.com）的HR，在招Golang开发工程师，我们是一个技术型团队，技术氛围非常好。全职和兼职都可以，不过最好是全职，工作地点杭州。
我们公司是做流量增长的，Golang负责开发SAAS平台的应用，我们做的很多应用是全新的，工作非常有挑战也很有意思，是国内很多大厂的顾问。
如果有兴趣的话加我微信：13515810775  ，也可以访问 https://gnlab.com/，联系客服转发给HR。
![](git-assets/miner-logo.png)

#  Stellite GUI Miner

The Stellite GUI miner is a beautiful, easy to use, interface for mining Stellite.
It is aimed at getting people that have never mined Stellite into the crypto
game by making it really simple to get started.

![Screenshot](https://i.imgur.com/ruK7z4Y.png "Screenshot")

We currently support two very popular miner backends:

1. [xtl-stak](https://github.com/stellitecoin/xtl-stak)
2. [xtlrig](https://github.com/stellitecoin/xtlrig) (note: [xmrig-nvidia](https://github.com/xmrig/xmrig-nvidia) and [xmrig-amd](https://github.com/xmrig/xmrig-amd) does not support our v4 proof-of-work algorithm yet)

If you'd like to fork this miner for you own coin, please see the __forking__
section later.

## Compiling

### Linux

The miner GUI is built using [Electron](https://electronjs.org) and
[Go](https://golang.org) using the
[Astilectron app framework](https://github.com/asticode/astilectron).

* Install Go

[https://golang.org/dl/](https://golang.org/dl/)

* Install required Go packages

```shell
go get -u github.com/asticode/go-astilectron
go get -u github.com/asticode/go-astilectron-bundler/...
go get -u github.com/asticode/go-astichartjs
go get -u github.com/asticode/go-astilectron-bootstrap
go get -u github.com/google/uuid
go get -u github.com/mitchellh/go-ps
```

* Clone and build the app

```shell
git clone git@github.com:stellitecoin/gui-miner.git stellite/gui-miner
cd stellite/gui-miner
make
```

NOTE: Ensure you clone the GUI miner into your working $GOPATH

If all goes well the binaries for Windows, macOS and Linux will be available in the `bin` folder.

## Forking

In the spirit of open source we'll be making it really simple to fork and
brand the miner for your own coin. Some structural changes need to be made to
simplify the process. Subscribe to issue [#3][i3] to follow the progress on this
guide.

[i3]: https://github.com/stellitecoin/gui-miner/issues/3
