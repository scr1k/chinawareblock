# 更新日志： Alpha--------------------------03/29/2020：更新一下证书



# chinawareblock
国产流氓、娱乐软件和不受欢迎的软件屏蔽工具
其实是个很菜的东西


# 制作背景
* 妹妹的电脑总被安装一些奇怪的流氓软件，所以我打算写一个免疫流氓软件的程序，看了看发现好像别人已经写过了，就是证书太旧了，需要更新，而且有些软件连个证书都没有，所以决定在"chinawareblock"的基础上进行修改一下。


# 使用要求和限制

* 需要Vista以上系统，需要UAC开启
* 软件也要有点级别，对于那些连数字证书都没有的产品，会创建一个禁止读写的文件夹来进行处理。

* 据说配置非常差的电脑不建议拉黑太多证书 （我试了一下好像没有影响）

# 使用方法

* 最简单粗暴的方法，把工具随便解压在哪里，双击运行**除腾讯全拉黑.bat**，会拉黑子文件夹下所有证书相关的软件。腾讯文件夹下的不敢拉黑，不然这电脑没人用了，腾讯你牛逼。
* 也可以单独进一个个文件夹，点击**~一键拉黑.bat**，拉黑文件夹下所有证书。证书可以根据需要自行增减。
* 证书文件的命名方式是公司名-软件名-加密方式-到期日，所以如果到期日已经过了的证书，应该要留一下他们新的安装包，可能要补充新的拉黑了。

# 证书提取工具
* 感谢@EraserKing网友提供的C#程序和@rewqazxv网友提供的Powershell脚本，提供了提取exe文件数字签名的功能，这样拉黑的操作就更简单了。用法：将一个或多个流氓exe放在本目录，双击运行GetCertFromFolder.exe，或者右键GetCertFromFolder.ps1，选择“使用PowerShell”运行，过一阵子全部证书文件就被导出来，可以拿去分类拉黑了，或者干脆就地拉黑~~~

# 需要扩充的功能
* 关于如何导出exe文件的全部证书，因为能力问题，只是找了下资料，然而没有去学习。先放这吧，免得有时间学的时候连资料都找不到了。https://www.sysadmins.lv/blog-en/reading-multiple-signatures-from-signed-file-with-powershell.aspx
