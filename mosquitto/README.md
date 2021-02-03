使用说明
----

把当前目录文件复制到`/home/mqtt`文件夹，文件结构如下:

```
/home/mqtt
        - config
            - mosquitto.conf
            - passwd
        - data
        - log
```

```bash
docker run -d --restart=always --name="mqtt" -p 1883:1883 -p 9009:9001 -v /home/mqtt:/mosquitto  eclipse-mosquitto:latest

```


密码生成
====
