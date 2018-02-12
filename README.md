# hexo + github
## 先下载此文件
然后打开文件中的hexo文件夹，并打开bash
下载npm的包,并下载主题文件（hexo只自动下载默认主题）
```
$ npm install
$ git clone https://github.com/luuman/hexo-theme-spfk.git themes/spfk

```
写文章
```
$ hexo new (文章名称)
```
编写完文章后,更新并开启服务器，本地查看格式问题
```
$ hexo generate
$ hexo server

```
若编写完毕，部署到给github上
```
$ hexo deploy
```
