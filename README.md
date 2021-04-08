### libuv中文教程 示例源码

libuv中文教程链接: <https://luohaha.github.io/Chinese-uvbook/index.html>

clone自: <https://github.com/nikhilm/uvbook>

libuv源码路径: <https://github.com/libuv/libuv>

#### linux下编译libuv方法

```shell
$ git clone https://github.com/libuv/libuv.git
$ cd libuv
$ cmake -H. -Bbuild # -DCMAKE_BUILD_TYPE=Debug
$ cmake --build build
```
