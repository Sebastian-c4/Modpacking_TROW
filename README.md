# Modpacking_TROW

**更新WeiDU版本至24600** *2018.09.10*

T.R.O.W. 专用模组打包工具
v1.0

诚邀各位Modder使用，将T.R.O.W.打造成中国的无限引擎游戏模组集散地！

本程序由 c4_angel 即 四是而非 修改自 ModPackaging: https://github.com/Gibberlings3/ModPackaging ，感谢原作者Mike1072 and CamDawg！
Banner图片制作：站长inthel

请于Windows系统下使用本工具。

———————————————————————————————————————————

使用说明：

1. 将下载得到的 ModPackaging_TROW.zip 解压缩后放置于任意目录下，目录名不可使用中文。

2. 将你制作的Mod（例如：MyMod）主文件夹放到 ModPackaging_TROW\Working 目录下（无须Setup-MyMod.exe）。至此，当前Working中应该包含：5个文件夹：audio、languages、style、tiz、MyMod；以及2个文件 package_mod.bat 和 desktop.ini。

3. 将style文件夹与desktop.ini复制一份，放入MyMod下，如已存在选择覆盖。

4. 根据你mod的情况选择将 languages 文件夹复制进MyMod。*注1。

5. 根据你mod的情况选择将 audio 和（或）tiz 文件夹复制进MyMod。*注:2。

6. 用任意文本编辑工具，推荐Notepad++打开Working目录下的package_mod.bat，根据文件内的注释对一些变量进行修改，然后保存退出。

7. 双击package_mod.bat运行，程序将根据你设定的变量生成最多3个安装包，分别对应Windows、OSX和Unix系统。

———————————————————————————————————————————

注1：languages文件夹中包含了使用WeiDU命令：HANDLE_CHARSETS 转码时需要的iconv程序。由于参数iconv_path的默认值是%tra_path%/iconv，故将iconv目录置于languages目录下，可在调用命令时无须单独设置iconv_path，具体请参阅WeiDU说明文档。如在mod中已将该文件夹放置于相同或不同的地方，或mod不支持增强版、不需要对文本进行转码则可跳过此步骤。

注2：audio文件夹下放置了导入音频所必须的oggdec.exe(win32) 和 sox(osx/unix)；而tiz文件夹下包含了用于不同系统的tisunpack程序（新增地图所必需）。如mod中并不包含新的音频、地图文件则可跳过此步骤。
