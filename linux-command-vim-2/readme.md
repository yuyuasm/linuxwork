1. /tmp 新建目录, 并进入

```bash
mkdir /tmp/mytest
cd /tmp/mytest
```

2. 复制 /etc/man_db.conf 到当前目录并用 vim 打开

```bash
cp /etc/man_db.conf .
vim man_db.conf
```

3. vim 设置行号，移动到 58 行，将光标右移 8 格

```bash
set nu
:58
l 8
```
4. 光标移动到第一行，向下查找 gzip

```bash
gg
/gzip
```

5. 50~100 行 man 大写，并且挨个问是否修改

```bash
:50,100s/man/MAN/gc
```

6. 修改后复原

```bash
u
```
7. 复制第 65~70，并粘贴至最后一行

```bash
:65
y5
G
p
```
8. 删除 23~28 开头为 # 的批注数据

```bash
:23
d5
```

9. 将这个文件另存为 man.test1.config

```bash
cp man_db.conf man.test1.confi
```
