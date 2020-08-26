# 英雄联盟竞技征召 Ban/Pick 系统

（2020.8.26立项，正在开发中）

## 总览

环境：Windows 10，中国大陆服务器（腾讯服）

本项目将使用 Python、 Riot Games 的游戏数据库及素材等工具，帮助业余英雄联盟比赛实现职业联赛所使用的 Ban/Pick 模式：竞技征召模式，即3ban、3pick、2ban、2pick。

本系统（以下简称BP系统）预计实现如下功能：

#### 服务端

1. **直接使用本地已登录的英雄联盟账号登录**，免去注册、登录等步骤，做真正一键登录的轻便工具
2. 实现多路复用，摒弃以前所使用的每个用户一个线程的大开销架构，支持更多人同时使用

#### 客户端

##### 管理员

1. 添加举办者账号
2. 对不合规的举办者、参赛者进行封号
3. 编辑或取消比赛

##### 举办者

1. 通过输入参赛人员ID、位置、名字、时间来创建比赛
2. 获得给观众使用的邀请码，使拥有邀请码的观众也能实时看到BP情况

##### 参赛者

1. 获取本地登录英雄联盟的ID，自动进入对应的比赛就位
2. 对房间内的英雄选择进行监督，确保阵容、英雄所使用玩家与BP系统中的相同，否则直接判负
3. 获取比赛结果并保存至服务器。要求任一参赛者上传rofl录像文件至服务器
4. 中场休息时间计时
5. **不太可能完成但是可以试一试的语音功能**

##### 观众：

1. 通过邀请码参与观看BP
2. 弹幕讨论



正在开发中，敬请期待。欢迎联系：baisebaoma@foxmail.com
