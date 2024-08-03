# DockerDesktop--
如何自己修改汉化
安装 Node.js 和 npm
npm是指node.js里面的
https://nodejs.org/zh-cn 

需要设置终端代理
set http_proxy=http://127.0.0.1:7890
set https_proxy=http://127.0.0.1:7890

目录
右键Docker Desktop图标，打开文件所在的位置
找打app.asar

安装asar
npm install -g @electron/asar

解压
asar extract 你的文件名字.asar ./解压文件夹名字
(最好是在asar的原始文件目录解压，)
cd 到解压文件夹名字

过程
需要一个Visual Studio Code，(你需要知道要汉化的英文)
进行搜索即可

打包
cd ..
asar pack 解压的文件夹名字 自定义名字.asar

最后
替换原始app.asar文件，（建议，将原始文件重命名，不要删除）
