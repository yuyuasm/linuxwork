1. at 设置定时，2 分钟后发送 hello, lxl. 20 分钟后重启系统
```bash
 echo 'wall "hello, lxl"' | at now +2 minutes
 echo 'reboot' | at now +2 minutes
```

2. crontab 定时任务， 每小时 30 min 将 /home 打包为 lxl.tar.gz

```bash
crontab -e
30 * * * * tar czf /lxl.tar.gz /home
crontab -l
```
