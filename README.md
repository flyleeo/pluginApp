# pluginApp
插件化
	
  
  Suming这是一个加载插件的宿主APP 它可以跳转类名为com.lee.test.TestActivity的apk  

	这个apk写好apk时放到储存卡的根目录  并把apk命名为 app-debug.apk

	总的来说  可以加载 名字app-debug.apk  且里面有com.lee.test.TestActivity 这个类的apk  但不能引用布局 图片等.

可以在acitivity中写布局 setcontentview(view); 

	加载布局的插件app
	
	将PluginActivity 和PluginResources 放到插件APP中   activity继承PluginActivity 不需要manifest声明
	
	加载布局 只需将布局名称 设置到setContentName("布局名称")

	初始化控件调用 findViewByName("控件名称")

	获取图片可用 getDrawable("图片名称")

	示例可看 TestActivity
