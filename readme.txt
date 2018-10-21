使用IrisSkin4的步骤：
1. 将IrisSkin4.dll动态文件导入当前项目引用中。具体操作为：解决方案资源管理器->当前项目->引用->右键->添加引用，找到IrisSkin4.dll文件，然后加入即可。建议，最好把IrisSkin4.dll文件放在当前项目\bin\Debug文件中。

2. 然后把IrisSkin4.dll文件添加到VS2010的工具箱：视图->工具箱->右键->选择项->浏览找到IrisSkin4.dll文件(文件最好放在当前项目\bin\Debug文件中）按确定，控件就添加到工具箱中了，然后把工具箱中新添加的 SkinEngine控件拖到当前项目中。

3. 把皮肤目录中的.ssk文件复制到当前项目\bin\Debug文件中，ssk文件可以根据需求自己选择.

4. 再在项目中调用.ssk皮肤文件。例：

   在自己的主程序的MainForm窗口对应的 MainForm.Designer.cs中，先声明private Sunisoft.IrisSkin.SkinEngine skinEngine1;然后是在InitializeComponent()  （Windows 窗体设计器生成的代码）定义