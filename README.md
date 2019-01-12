声明：
  该工具是song0071000提供的，项目git地址：https://github.com/song0071000/unpack_plist_png 。感谢song0071000。
  我这里fork下来，是因为我在安装使用该工具的过程中，遇到了些问题（因为我不会python，也暂没有计划学习python.），我总结了以下使用步骤，保证了自己下次能拿来就用，一次ok。这里再次感谢song0071000 . 
    
使用步骤：  
  该工具只能运行在windows环境中，我windows7测试已通过。  
  1. 安装python2.7(必须是2.7，因为该工具是开发语言是python2.7。如果是3.x，会出现编译错误，无法提取。 建议官网下载python(python官网地址https://www.python.org/downloads/windows/)。注意，电脑已经安装了python2.7,需要核查下python2.7安装目录/Scripts文件夹下是否有pip.exe和pip2.exe,没有pip*.exe则需重装python2.7；
  2. python安装好后，需要设置环境变量Path：添加python27的安装目录\;python27的安装目录\Scripts；
  3. 打开cmd，执行 python -m pip install --upgrade pip 命令完成pip的更新升级。再执行 pip install Pillow 命令完成pillow的安装（最好这样做，如果你要安装离线软件包，那你先要熟悉python【不是说你会拼写python，就可以了】。）；
  4. Put "unpack_plist.py" script file in the same directory with plist and png files.（这句话说得很好，我就不改动了）；   
  5. 打开cmd，执行python unpack_plist.py 图集名 （注意：这里 “图集名”，不要加文件类型后缀。）。
  6. ok了。

##Example
  if the current directory has files "unpack_plist.py" "MessageImage.plist" and "MessageImage.png", the only work you should do is typing the follow command: python unpack_plist.py MessageImage. Then the tiny png files are made.


