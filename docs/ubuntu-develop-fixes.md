# 1
### Error: Running "exec:linux64"

```
Running "exec:linux64" (exec) task
>> Exited with code: 127.
>> build/cache/linux64/0.9.2/nw: error while loading shared libraries: libudev.so.0: cannot open shared object file: No such file or directory
Warning: Task "exec:linux64" failed. Use --force to continue.
```
### Solution:
```sudo ln -sf /lib/x86_64-linux-gnu/libudev.so.1 /lib/x86_64-linux-gnu/libudev.so.0```
