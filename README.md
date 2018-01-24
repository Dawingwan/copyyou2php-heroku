`git clone https://github.com/You2php/you2php-heroku.git`
`cd you2php-heroku`
`heroku create {You APP Name}`
`git push heroku master`
`heroku ps:scale web=1`
`heroku open`

陆续执行这些命令就可以了。{You APP Name}改成您的应用域名前缀名（不需要加花括号）。
首页显示空白，一般是mbstring库没有开启导致了，建议官方的文档开启mbstring.
首页空白不影响使用，搜索和播放功能正常，
由于heroku会自动重置，可能会导致应用过了一段时间会还原到安装前状态，建议您先在本地搭建php环境安装you2php，然后把安装后的you2php所有文件push到您的heroku应用。
