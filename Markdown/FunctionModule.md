```text
title: FunctionModule
date: 2019-06-24 18:03:31
```







# 功能代码块



## 获取 cmd 执行后的文本结果

### Java
这个类已经被单独封装, 可以移植到其他计算机上使用, 只需要接收一个字符串数组即可.</br>
```java
new cmdStrCommand(new String[]{"cmd","/C","type","C:\\Windows\\System32\\drivers\\etc\\hosts"}).ConsoleTerminalAscii();
```
功能代码块:</br>
```java
import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStream;
import java.io.InputStreamReader;

public class cmdStrCommand {
    private String cmd[];
    public cmdStrCommand(String cmd[]){
        this.cmd = cmd;
    }

    public void ConsoleTerminalAscii(){
        Process cmdStr;
        try{
            cmdStr = Runtime.getRuntime().exec(cmd);
            InputStream inputStream = cmdStr.getInputStream();
            InputStreamReader inputStreamReader = new InputStreamReader(inputStream);
            BufferedReader bufferedReader = new BufferedReader(inputStreamReader);
            String line = null;
            while ((line = bufferedReader.readLine()) != null)
                System.out.println(line);
        }
        catch (IOException e){
            e.printStackTrace();
        }
    }
}
```



## 模拟系统启动并自动登录流程

### Java

调用代码:</br>
```java
new ProgramHead().getProgramHead();
```
功能代码块:</br>
```java
public class ProgramHead {

    public static void getProgramHead(){

        System.out.println("\"I am Very Busy [版本: 1.0.0_512]\"");
        System.out.println("(c) 2019-06-04 作者: StringOD. 保留所有权利");
        System.out.println();
        OutTime.setLongOutTime();

        OutTime.setLongOutTime();
        System.out.println("BIOS自检..........................................完成");
        OutTime.setLongOutTime();
        System.out.println("加载硬盘...........................................26%");
        OutTime.setLongOutTime();
        System.out.println("加载硬盘...........................................57%");
        OutTime.setLongOutTime();
        System.out.println("加载硬盘...........................................完成");
        OutTime.setLongOutTime();
        System.out.println("读取引导文件........................................完成");
        OutTime.setLongOutTime();
        System.out.println("加载StringOD内核...................................完成");
        OutTime.setLongOutTime();
        OutTime.setLongOutTime();
        System.out.println("启动str进程........................................完成");
        OutTime.setLongOutTime();
        System.out.println("启动内核模块........................................完成");
        OutTime.setLongOutTime();
        OutTime.setLongOutTime();
        System.out.println("执行/Users/HiWin10/Desktop/TeLuoYiMuMa.exe.........完成");
        OutTime.setLongOutTime();
        OutTime.setLongOutTime();
        System.out.println("启动StrGUI.....完成");
        OutTime.setLongOutTime();

        System.out.println("执行自动登录脚本");
        OutTime.setShortOutTime();

        for (int i = 0; i < 10; i++)
            System.out.print("▃");
        System.out.println();
        String user = "账户: ";
        System.out.print(user);
        OutTime.setSuperShortOutTime();
        System.out.print("S");
        OutTime.setSuperShortOutTime();
        System.out.print("t");
        OutTime.setSuperShortOutTime();
        System.out.print("r");
        OutTime.setSuperShortOutTime();
        System.out.print("i");
        OutTime.setSuperShortOutTime();
        System.out.print("n");
        OutTime.setSuperShortOutTime();
        System.out.print("g");
        OutTime.setSuperShortOutTime();
        System.out.print("O");
        OutTime.setSuperShortOutTime();
        System.out.println("D");
        OutTime.setSuperShortOutTime();

        String password = "密码: ";
        System.out.print(password);
        OutTime.setSuperShortOutTime();
        System.out.print("*");
        OutTime.setSuperShortOutTime();
        System.out.print("*");
        OutTime.setSuperShortOutTime();
        System.out.print("*");
        OutTime.setSuperShortOutTime();
        System.out.print("*");
        OutTime.setSuperShortOutTime();
        System.out.print("*");
        OutTime.setSuperShortOutTime();
        System.out.print("*");
        OutTime.setSuperShortOutTime();
        System.out.print("*");
        OutTime.setSuperShortOutTime();
        System.out.print("*");
        OutTime.setSuperShortOutTime();
        System.out.println("*");
        OutTime.setSuperShortOutTime();
        for (int i = 0; i < 10; i++)
            System.out.print("▃");
        System.out.println();

        System.out.println("欢迎访问\"I am Very Busy!\"");
        OutTime.setLongOutTime();
        System.out.println("程序启动");
        OutTime.setLongOutTime();

    }
}
```



## 打开文件

### Java
```java
			//打开本地程序文件方式1
			Runtime rt = Runtime.getRuntime();
			String fileLac = "D:\\HBuilder\\HBuilder.exe";
	        rt.exec(fileLac);
		======================================
	        //打开本地程序文件方式2
		try {
	        Desktop desktop = Desktop.getDesktop();
	        File file = new File("C:\\Users\\HiWin10\\Desktop\\勇者之路精灵物语速升版.html");
	        desktop.open(file);
		}
		catch(IOException e) {
			System.out.println("文件不能被打开");
		}
		======================================
	        打开本地网站，默认浏览器打开
		try {
	        URI uriNet = new URI("C:\\Users\\HiWin10\\Desktop\\勇者之路精灵物语速升版.html");
	        Desktop.getDesktop().browse(uriNet);
		}
		catch(URISyntaxException e) {
			System.out.println("URI地址错误");
		}
		catch(IOException e) {
			System.out.println("文件不能被打开");
		}
```



## 调用Flash文件

### HTML
```html
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8" />
		<meta name="viewport" content="width=device-width, initial-scale=1">
		<title></title>
	</head>
	<body>
	<embed src="C:\Users\HiWin10\Desktop\game2.swf" width="1024" height="800"></embed>
	</body>
</html>
```



## 添加菜单

### Android
```java
public boolean onCreateOptionsMenu(Menu menu){
	getMenuInflater().inflate(R.menu.main,menu);
	//显示菜单
	return true;
}
```



## 添加菜单项

### Android
```java
public boolean onOptionsItemSelected(MenuItem menuitem){
	        switch (menuItem.getItemId()){
            case R.id.menu_item_add:
                Toast.makeText(MainActivity.this,"A",Toast.LENGTH_SHORT).show();
                break;
            case R.id.menu_item_remove:
                Toast.makeText(MainActivity.this,"B",Toast.LENGTH_SHORT).show();
                break;
            case R.id.menu_item_StringOD:
                Toast.makeText(MainActivity.this,"C",Toast.LENGTH_SHORT).show();
                break;
            default:
                break;
        }
	//显示菜单项
	return true;
}
```

