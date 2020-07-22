# WaymarkLibrarian-CN
----------
# 目的
----------
这是一个为最终幻想XIV提供的工具，允许玩家将无限数量的标点预设替换游戏内游戏提供的极为有限的标点插槽，使用这个程序的风险由你自己承担（请阅读下面的重要部分）。  
原作者版：https://github.com/PunishedPineapple/WaymarkLibrarian  
国服适配：CillinjoLo 西林觉罗西瓜  
技术支持：Bluefissure獭爹和加隆德青磷技术开发部的所有成员  

----------
# 基本使用方法
----------
1.获取最新版本程序https://github.com/CillinjoLo/WaymarkLibrarian-CN/releases
  Newtonsoft.Json.dll需要跟程序本身在同一个文件夹（这个dll允许导入和导出预设）  
2.第一次运行程序时，系统会提醒您备份角色设置，然后再继续。也可能会提示您有可用的更新文件。  
  如果不更新的话程序将运行而不更新这些文件，但它可能无法写入预设游戏或显示区域名称。  
3.选择FFXIV存储用户配置文件的文件夹。程序在第一次启动时地址为“…\Documents\My Games\FINAL FANTASY XIV-Realm Reborn”，  
  国服的话在 游戏根目录\game\My Games\FINAL FANTASY XIV - A Realm Reborn,可以单击“…”按钮进行更改。  
4.选择要查看/编辑其预设的角色。有关角色名的详细信息，请参阅下面的别名部分。  
  另外请注意，如果角色最近没有登录，程序将弹出一条消息，说明它无法读取路标预设。如果发生这种情况，只需登录并注销该角色，以获得程序可以读取的文件。  
5.现在，您可以在左侧列表中为该角色选择五个预设插槽中的任何一个，然后查看预设信息、删除它或将其复制到库中。  
6.库和游戏是完全分开的。您可以在库中存储无限数量的标点预设，并且这些预设可以具有描述性名称（例如，e7s PUG Strats、e7s Static Strats、e7s Uptime、UCoB Inversed、UCoB Vertical等）。玩家的数据完全与库分开存储。  
7.在库中有预设后，可以使用“<-复制到游戏”按钮将其复制到选定的角色。这会将选定的预设从库复制到选定的游戏槽。请注意，这还不会影响游戏内的预设。  
8.一旦您对角色的五个预设槽修改完成，您必须单击“写入游戏文件”按钮，更新的预设将反映在游戏中。另请注意，写入该文件，该所选角色必须注销。如果角色已经登录时你点击写入按钮，游戏将覆盖你所做的任何更改。   

----------
# 导入、导出和编辑预设
----------
该程序允许您导入其他人创建的预设，以及为其他人导出您自己的预设。如需导入，请单击库下面的“导入”按钮并粘贴固定格式的数据。导入的格式还接受Paisley Park预设，尽管您必须手动设置并保存区域ID，因为Paisley Park不存储或提供该信息。要导出预设，只需单击库下面的“导出”按钮并复制所提供的文本。  
您还可以编辑库中任何预设的名称、区域和路标位置。为此，请在库中选择所需的预设，输入/编辑程序右侧的字段，然后单击底部的“更新”按钮。

----------
# 重要！
----------
这个程序应该被认为是测试版。到目前为止，它只是用少数几个角色进行了测试，而且由于路标格式是逆向工程的，所以没有办法百分之百地确定它的编写是完美无缺和无法检测的。也就是说，游戏使用的数据格式非常简单，所以不会有太多错误。此外，虽然该程序不影响游戏可执行文件、内存等，但从技术上讲，SE可以通过以下两种方式之一检测该程序的使用：  
1.他们可以审核你的角色在标点预设显示保存时的位置，然后看到你当时不在相应的区域。  
2.他们可以为角色上的每个插槽保存一个并行的服务器端预设，并对照用户配置中保存的客户端预设进行检查。  
不过，这两种方法似乎都不太可能，因为它们会给任何将用户配置数据从主角色复制到其他角色的人带来误报，而且这些方法似乎比SE在将预设数据作为角色配置的一部分时所投入的工作量要多。

----------
# 别名
----------
默认情况下，角色名是混乱的数字和字母字符串，例如“FFIXV_CHR…”。单击“设置别名”并输入您容易记住的内容（即“角色名（服务器）”，将使该角色的名称出现在列表中。不幸的是，您必须手动确定哪个文件夹对应于哪个角色。我知道有两种方法可以做到这一点：  
1.确定哪个文件夹属于某个角色的最基本方法是登录到该角色，更改库存中的项目顺序，更改用户宏、热键栏等，重新注销，然后找出哪个文件夹包含在您注销时修改的文件。  
2.使用快速启动程序：https://github.com/goatcorp/FFXIVQuickLauncher（非官方），通过安装角色同步插件并在登录时检查配置页面。（不知道国服是否支持）  

----------
# 协议
----------
Code and executable are covered under the MIT License. Final Fantasy XIV (and any associated data used by this program) is copyright Square Enix.
