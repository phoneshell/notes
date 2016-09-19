# 安装输入法

##搜狗拼音输入法LINUX版官方下载[：http://pinyin.sogou.com/linux/?r=pinyin](：http://pinyin.sogou.com/linux/?r=pinyin)

###一、添加fcitx的nightlyPPA
用ctrl+alt+t唤出终端中，输入：
sudo add-apt-repository ppa:fcitx-team/nightly
sudo apt-get update
###二、安装fcitx，搜狗输入法附加组件
打开软件中心，搜索fcitx，然后安装Fcitx中文输入法，如下图（已经安装好了，默认会自动安装其他所需要的软件包）。然后再次搜索fcitx-sogoupinyin，然后安装该搜狗输入法附加组件。
接着打开 设置》语言支持，将fcitx设置为默认键盘输入法
安装完毕后需要注销，然后重新登陆即可生效。
也可以安装其他输入法附加组件，如fcitx-googlepinyin，fcitx-module-cloudpinyin，fcitx-sunpinyin。
###三、如果安装后出现无法启动输入法，则按照如下方法重新操作
首先按上述方式打开终端，执行如下命令卸载fcitx和ibus
sudo apt-get remove fcitx
sudo apt-get remove ibus
sudo apt-get autoremove
然后打开软件中心，搜索fcitx和ibus，将其中有关的软件包删除干净，然后打开Ubuntu Tweak（需要另外安装）使用清道夫将不需要的软件包，软件配置文件等清理干净，再重新安装fcitx和fcitx-sogoupinyin，注销后重新登陆即可。
