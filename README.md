# go2csp
正在开发中....

Go 语言并发编程中可以使用管道的方式进行进程间通信，这种方式是借鉴了 CSP 的思想

本工具可以将 Go 语言 使用管道通信的方式的编程的程序，自动化运行得到 CSP 脚本，可以使用 PAT 等模型验证工具进行验证，得出所实现的 Go 程序中是否有死锁等性质的验证工作。

## 使用

如 example 中，调用 CSP 包中对 go 原有并发库进行封装后的并发函数进行并发编程。

运行时，如果没有参数，那么就是正常运行，可以加参数

```
go run xxx.go -csp <xxx.csp>
```

输出文件名是可选参数，默认为 main.csp.