1. 登录

```bash
su yuyu
cd ~
```

2. 创建 test4, 并查看

```bash
mkdir -p test4
ls test4

```
3. 创建 hello-lxl

```bash
touch hello-lxl
```
4. vim edit hello-lxl

```bash
vim hello-lxl
fafuhaoijfoiaoaafjalfalkfjaljflaalfjjajfa
yy
50p
```
5. wc hello-lxl

```bash
wc hello-lxl
```
6. 查看 hello-lxl

```bash
cat hello-lxl
```

7. 复制 /etc/passwd test4/lxl-copy

```bash
cp /etc/passwd test4/lxl-copy
```

8. 查看头 2 尾 8

```bash
head -2 test4/lxl-copy
tail -8 test4/lxl-copy
```

9. 移动 hello-lxl 到 test4

```bash
mv hello-lxl test4/
```

10. 递归查看主目录

```bash
ls -la -R ~
```
11. 递归复制 test4 到 dir

```bash
cp -r tests/ dir/
```

11. 删除 test4
```bash
rm -rf  test4
```

10. 递归查看主目录

```bash
ls -la -R ~
```
