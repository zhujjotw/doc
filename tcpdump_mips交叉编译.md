
### 编译libpcap
```
./configure --host=mips-linux-gnu --with-pcap=linux
make
make clean
```

### 编译tcpdump
```
./configure --host=mips-linux
make
make clean
```

### mips-gnu编译需要在Makefile添加如下选项
```
CFLAGS+=-mips32r2
CFLAGS+=-muclibc
```