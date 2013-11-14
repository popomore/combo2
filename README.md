# Combo2

A simple assets combo server.

---

## Feature

1. 支持单文件访问
1. 支持 combo 访问，combo 的格式为(/??a.js,b.js)
1. 支持远程代理，如果本地不存在会去远程的地址找
1. 支持缓存，如果从远程获取的文件会缓存到本地

## Install

```
$ npm install combo2 -g
```

## Usage

启动服务

```
$ cd path/to/directory
$ combo
```

指定根目录，可在任意目录执行命令

```
$ combo -d path/to/directory
```

代理远程文件，默认开启缓存 

```
$ combo -r http://a.alipayobjects.com
```

## Options

- `-v, --verbose` 显示访问日志
- `-p, --port [port]` 指定服务器端口
- `-d, --directory [directory]` 指定根目录
- `-r, --remote [remote]` 指定远程地址，如果本地不存在会去远程找

## Lisence

MIT
