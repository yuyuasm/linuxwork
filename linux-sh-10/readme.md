1. 输入数字，累加求和

```bash
#!/usr/bin/bash

read -p 'input num: ' num

cnt=0
i=0
while [ $i -le $num ];
do
    cnt=$(($cnt+$i))
    i=$(($i+1))
done
echo $cnt
```

2. /root/test/logica 

```bash
#!/usr/bin/bash
name="/root/test/logica"
if [[ ! -e $name ]];
then
    mkdir -p "/root/test/logica"
    touch $name
    exit 0
fi

if [[ -f $name ]]
then
    rm $name
    mkdir $name
    exit 0
fi

if [[ -d $name ]]
then
    rm -rf $name
    exit 0
fi
```
3. 输出 /etc/passwd

```bash
#!/usr/bin/bash

cat /etc/passwd -n | grep ":" | sed "s/:/ /g" | awk '{print "The " $1 " account is " $2}'
```
