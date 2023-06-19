### oom日志查看
```bash
sudo egrep -i -r 'killed process' /var/log
sudo dmesg
```

### linux查看符号表和地址
- 查看符号表:
```bash
readelf -s <文件名>
```

- 查看地址:
```bash
readelf -a <文件名>
```

- 如果想要更详细的信息,可以使用 -w 参数,如:
```bash
readelf -w -a <文件名>
```

- 如果想要查看可执行文件中的符号表和地址,可以使用objdump命令:
```bash
objdump -t <可执行文件名>
```

- 还可以使用-d参数来查看可执行文件中的汇编代码
```bash
objdump -d <可执行文件名>
```
