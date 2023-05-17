![logo-blue](https://user-images.githubusercontent.com/51039935/197520391-f35db354-6071-4c12-86ea-fc450f04bc85.png)
# NAS媒体库管理工具

[![GitHub stars](https://img.shields.io/github/stars/wzzqq/my-nastools?style=plastic)](https://github.com/wzzqq/my-nastools/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/wzzqq/my-nastools?style=plastic)](https://github.com/wzzqq/my-nastools/network/members)
[![GitHub issues](https://img.shields.io/github/issues/wzzqq/my-nastools?style=plastic)](https://github.com/wzzqq/my-nastools/issues)
[![GitHub license](https://img.shields.io/github/license/wzzqq/my-nastools?style=plastic)](https://github.com/wzzqq/my-nastools/blob/master/LICENSE.md)
[![Docker pulls](https://img.shields.io/docker/pulls/jxxghp/nas-tools?style=plastic)](https://hub.docker.com/r/jxxghp/nas-tools)
[![Platform](https://img.shields.io/badge/platform-amd64/arm64-pink?style=plastic)](https://hub.docker.com/r/jxxghp/nas-tools)


Docker：
* https://hub.docker.com/r/jxxghp/nas-tools 
* https://hub.docker.com/r/nastool/nas-tools

TG频道：https://t.me/nastool_official

Wiki：https://wiki.nastool.cn

API: http://localhost:3000/api/v1/


## 功能：

NAS媒体库管理工具。


## 安装
### 1、Docker
```
docker pull jxxghp/nas-tools:latest
```
教程见 [这里](docker/readme.md) 。

如无法连接Github，注意不要开启自动更新开关(NASTOOL_AUTO_UPDATE=false)，将NASTOOL_CN_UPDATE设置为true可使用国内源加速安装依赖。

### 2、本地运行
python3.10版本，需要预安装cython，如发现缺少依赖包需额外安装：
```
git clone -b master https://github.com/wzzqq/my-nastools --recurse-submodule 
python3 -m pip install -r requirements.txt
export NASTOOL_CONFIG="/xxx/config/config.yaml"
nohup python3 run.py & 
```

### 3、可执行文件
下载打包好的执行文件运行即可，会自动生成配置文件目录：

https://github.com/wzzqq/my-nastools/releases

### 4、群晖套件
添加矿神群晖SPK套件源直接安装：

https://spk.imnks.com/

https://spk7.imnks.com/

## 免责声明
1) 本软件仅供学习交流使用，软件本身不提供任何内容，仅作为辅助工具简化用户手工操作，对用户的行为及内容毫不知情，使用本软件产生的任何责任需由使用者本人承担。
2) 本软件代码开源，基于开源代码进行修改，人为去除相关限制导致软件被分发、传播并造成责任事件的，需由代码修改发布者承担全部责任。本项目的用户认证机制是项目长期生存下去的基础，建议不要修改用户认证并公开发布。
3) 本项目没有在任何地方发布捐赠信息页面，也不会接受捐赠或进行收费，请仔细辨别避免误导。