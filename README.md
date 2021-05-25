# Chia Blockchain FAQ

奇亚 区块链 常见问题

不定时更新,仅供参考

## 绘图文件不可用
说明: 钱包中显示绘图(plots)文件状态为不可用

以Windows  1.1.6 版本 钱包为例:

解决方案:

1.关闭钱包

2.cmd 输入(根据版本号进行变动) 

```cmd
##dir 显示当前路径所有文件
cd %LocalAppData%\chia-blockchain
cd app-1.1.6
cd resources
cd app.asar.unpacked
cd daemon
##添加绘图文件路径(plots)
chia.exe   plots add -d 文件路径
#chia.exe  plots add -d e:\plots\
#如有多个就执行多个 chia.exe   plots add -d  
```
3.重新打开钱包

## 加速节点同步
说明: Chia节点同步过慢

解决方案:

下载 https://github.com/Pow-Duck/ChiaNodeSyncing/releases/

或自行编译ChiaNodeSyncing 


QQ交流群: 816250346
