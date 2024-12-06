1. 切换 root

```bash
su
```

2. 添加用户 userlxl, 并设置密码

```bash
useradd userlxl -p qwer1234
```

3. 添加用户 user2, 并设置密码, 并指定 uid

```bash
useradd user2 -u 1045 -p qwer1234
```

4. id 查看 userlxl user2

```bash
id userlxl
id user2
```

5. groups 查看 userlxl user2

```bash
groups userlxl
groups user2
```

6. 添加用户组 grp1 和 grp2

```bash
groupadd grp1
groupadd grp2
```

7. 将 userlxl 主组改为 grp1, 将 userlxl, user2 添加到 grp2

```bash
usermod -g -a userlxl grp1
gpasswd -a userlxl grp2
gpasswd -a user2 grp2
```

8. id 查看 userlxl, user2

```bash
id userlxl
id user2
```

9. groups 查看 userlxl user2

```bash
groups userlxl
groups user2
```

10. /etc/passwd 查看 userlxl user2,/etc/group 查看 grp1 grp2

```bash
cat /etc/passwd | less
cat /etc/group | less
```

11. grp2 删除 user2

```bash
gpasswd -d user2 grp2
```


12. groups 查看 user2

```bash
groups user2
```
