# my_node_tools
hello world!
bonjour!
https://github.com/alsotang/async_demo


node笔记

版本管理器：n模块
npm install -g n
n stable           升级node.js到最新稳定版
n latest            安装最新的版本
n 0.11.12         安装其他的版本
n rm 0.10.1      删除某个版本
n use 0.10.21 some.js    以指定的版本来执行脚本


npm使用：
npm -v          #显示版本，检查npm 是否正确安装。
npm install -g npm  /  npm i -g npm    更新npm至最新版本

npm install express   #安装express模块
npm install -g express  #全局安装express模块

npm show express     #显示模块详情
 
npm update        #升级当前目录下的项目的所有模块
 
npm update express    #升级当前目录下的项目的指定模块
npm update -g express  #升级全局安装的express模块
 
npm uninstall express  #删除指定的模块

npm list         #列出已安装模块
npm list -g --depth=0     #列出全局安装的模块
 
npm config get prefix
npm config set prefix



其他常用模块：
npm install -g yarnpkg
npm install node-mysql



node调试工具：
[console调试]
node debug debug.js

[远程调试]
一个终端中
$ node --debug-brk debug.js
debugger listening on port 5858
另外一个终端中
$node debug 127.0.0.1:5858
connecting... ok


页面调试：
[node-inspector]
1.安装：npm install -g node-inspector
2.node --debug-brk=5858 debug.js
3.在另一终端执行node-inspector 获取debug地址
Node Inspector v1.1.2
Visit http://127.0.0.1:8080/?port=5858 to start debugging.
4.在浏览器中打开 http://127.0.0.1:8080/?port=5858
*用n工具切换到6.5.0版本node可以正常安装 其他会报错
*node-pre-gyp install --fallback-to-build 卡住 执行npm install -g node-gyp

更改镜像地址：
npm config set registry https://registry.npm.taobao.org

库
underscore
async
promise
