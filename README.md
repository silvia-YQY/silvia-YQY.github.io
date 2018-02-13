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

重新上传到hexo分支

添加本地所有文件到仓库：
`git add -A`

添加commit：
`git commit -m "blog源文件"`

添加本地仓库分支hexo：  //此步骤为第一次是做，由于已经设定为hexo分支为主分支，故第二次开始不需要
`git branch hexo`

添加远程仓库：
`git remote add origin git@github.com:silvia-YQY/silvia-YQY.github.io.git.`

同步本地仓库到远程
`git push origin hexo`

这样就生成静态网页部署到了github中,并且源文件也上传到hexo分支上面


**此处有一个问题，每次上传源文件的时候，第三方主题的文件总是无法上传。故每次更新博客都需要下载重新手动主题，并修改主题配置**


[多终端配置](https://righere.github.io/2016/10/10/install-hexo/)
