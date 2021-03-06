# 新手入门指南


## Mac OS

#### 更新系统
Mac OS X 10.11.1

#### 安装 Xcode
* Xcode
* Xcode commandline tools

#### 常用系统工具安装
带*号的是必须安装，其他推荐

* [*] 安装 brew 工具，参考 http://brew.sh
* 编辑器，推荐 Vim/Emacs/Sublime Text 3
* Terminal: iTerm
* shell: oh-my-zsh
* [*] 用 brew 安装 git, python
* [*]用 pip 安装 virtualenv

## Python 环境配置

使用 virtualenv 配置虚拟环境

## github 使用

1. 注册 github 帐户；
2. 创建一个新项目；
3. 添加一个 README.md 文件，并提交到项目中。

## Python 小试牛刀

算法答题完成 Leetcode #1, #2, #3

要求：

1. 使用 Python 语言并通过；
2. 提交到之前的 github 项目中。

#### Python 语言学习参考

1. [Python 精要参考](http://wiki.woodpecker.org.cn/moin/WeiZhong/2006-01-17)
2. [Python 入门指南](http://www.pythondoc.com/pythontutorial3/)
3. [The Python Tutorial](https://docs.python.org/2.7/tutorial/index.html)

## 编辑器 VIM 使用

学习 Vim 的基本操作，完成一下步骤：

1. 编辑一个新文件；
2. 增加内容；
3. 编辑、删除内容；
4. undo/redo；
5. 保存退出；
6. 再编辑不保存退出。

## MySQL 环境准备
1. 在 mac 上用 `brew` 安装 MySQL；
2. 创建数据库，名称为 `reformation_development`；
2. 创建数据库用户，并赋予该用户 `reformation_development.*`的权限；
3. 用 `mysql` 命令登录数据库，测试数据库的连通性。

## Nginx 环境准备
1. 在 Mac 上使用 `brew` 安装 NGINX；
2. 修改 nginx 的配置，将 `location /`更改为你的静态文件目录；
3. 配置 /api 等的路径，为动态转发请求；
4. 启动、停止、重启 nginx 服务。

参考：[简明 VIM 练级攻略](http://coolshell.cn/articles/5426.html)
## Linux 环境

1. 生成密匙，包括公钥、私钥；密匙长度4096位
2. 使用密匙提交 github 代码
3. 配置.ssh/config，使用私钥登录开发服务器
4. 使用 virtualenv 配置自己的 python 虚拟环境
5. 使用 SimpleHTTPServer 模块运行一个 HTTP 服务，并在本地（mac 机器）下载一个文件

## Flask 入门

目标：

实现一个 API 服务器，实现查询美元对人民币汇率。

接口要求：

    GET /api/rate
        Response data sample:
            {'RMB_to_USD_rate': '0.16'}
    POST /api/rate
        Request data sample:
            {'RMB': '233.00'}
        Response data sample:
            {'USD': '36.42'}
        以及相对的，通过 USD 查询 RMB
