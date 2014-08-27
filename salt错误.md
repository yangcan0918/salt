# salt错误

### 执行salt '*' state.highstate命令报错

`salt '*' state.highstate`

```
 TypeError encountered executing state.highstate: 'bool' object is not iterable. See debug log for more info.  Possibly a missing arguments issue:  ArgSpec(args=['test', 'queue'], varargs=None, keywords='kwargs', defaults=(None, False))
 
```
解决办法：
  通过排查，发现服务端和客户端的版本不同，更新salt版本，使其一致即可