# 如何将C++绑定至Lua

两种方法可以将C++类/成员函数绑定至Lua。

1. 编写.pkg文件然后使用tolua++创建.h/.cpp文件如LuaCocos2d.h/.cpp

	.pkg文件跟.h文件一样会列出所有类和函数，格式请参见“$cocos2dDir/tools/tolua++/”中的文件。
	
2. 处理写.h/.cpp文件

为什么不使用pkg和tolua++？


static MyClass * createWithSize(CCSize s)


extern "C" {
