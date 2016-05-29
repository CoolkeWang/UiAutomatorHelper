# UiAutomatorHelper
UiAutomator 编译脚本

##使用方法:

#####1.UiAutomatorHelper.java放入到项目中去

#####2.写运行的main方法
```Java
public static void main(String[] args) {
		//new UiAutomatorHelper("Demo", "com.jikexueyuan.demo.Demo1", "testBrowser", "1");
		
		String workspase, className, jarName, androidId, sdkpath;
		workspase="C:\\Users\\fanhq\\git\\UiAutomatorHelper\\UiAutomatorDebug";
		className="com.jikexueyuan.demo.Demo1";
		jarName="demo1";
		androidId="1";
		sdkpath="E:\\Program Files (x86)\\Android\\android-sdk";
		CtsHelper cts=new CtsHelper(workspase, className, jarName, androidId, sdkpath);
		//cts.setDevices("0123456789");
		cts.runTest();
	}
```
#####3.运行这个main方法将会自动的生成jar包,并上传到手机进行相关的测试
