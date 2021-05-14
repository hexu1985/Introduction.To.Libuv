测试方法
1) 编译
2) 执行./main
3) 在另外几个窗口执行telnet 127.0.0.1 7000
4) 在开一个窗口执行`netstat -natp | grep 7000`能看到如下信息:
```
tcp        0      0 0.0.0.0:7000            0.0.0.0:*               LISTEN      32231/main      
tcp        0      0 127.0.0.1:52736         127.0.0.1:7000          ESTABLISHED 32238/telnet    
tcp        0      0 127.0.0.1:52740         127.0.0.1:7000          ESTABLISHED 32257/telnet    
tcp        0      0 127.0.0.1:7000          127.0.0.1:52736         ESTABLISHED 32235/worker    
tcp        0      0 127.0.0.1:7000          127.0.0.1:52740         ESTABLISHED 32234/worker
```
