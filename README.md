# mpv-remote

使用手机或者其它电脑控制mpv的播放。（例如你将kodi的默认播放器更改为mpv时，本身的kodi无法控制mpv)
### 安装

```sh
$ npm install
```
### 启动服务

```sh
$ node app.js {端口号}
```

不加端口号 默认3000
#### 可以使用pm2工具将服务加入开机启动

```sh
$ npm install -g pm2
$ pm2 start app.js
$ pm2 startup
$ pm2 save
```

### 启动mpv时带有input-ipc-server选项

```sh
$ mpv --input-ipc-server=/tmp/mpvsocket example.mp4
```


### 手机访问 http://ip:port 就可以使用遥控器了






License
----

MIT
