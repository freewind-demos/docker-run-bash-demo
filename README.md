Docker Run "bash" Demo
======================

```
$ docker run -it ubuntu bash
```

将会使用本机缓存中的`ubuntu`或者下载后执行，进入其`bash`:

```
root@010a01c556fb:/#
```

我们可以试一试：

```
root@010a01c556fb:/# pwd
/
root@010a01c556fb:/# ls
bin  boot  dev  etc  home  lib  lib64  media  mnt  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
root@010a01c556fb:/# uname
Linux
root@010a01c556fb:/#
```

关于参数
----

- `-i`: `--interactive`, 显示命令的输出
- `-t`: `--tty`, 显示命令提示符

如果不加`-i`，只会显示`root@010a01c556fb:/#`，而没有命令输出；
如果不加`-t`，命令的输出正常，但是没有`root@010a01c556fb:/#`

