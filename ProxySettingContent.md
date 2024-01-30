在WSL或者虚拟机中，我们通常会使用 git commit 来下载安装数据包，但是这里有一个问题，就是主机虽然启用了代理，然而虚拟机或者WSL里面的Linux系统在 git commit 的时候却会卡在传输指令的那一步（这个现象在NAT模式下尤为常见），使用 if config 指令我们可以查看到主机和虚拟机是在同一个IP地址上的（NAT模式不幸中的万幸）。那么这个时候，git就会默认不走代理，我们就需要给git单独设置代理模式。
下面这个网站可以帮到你：https://ericclose.github.io/git-proxy-config.html
记得给个Star  :)