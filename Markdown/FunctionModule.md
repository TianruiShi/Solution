```text
title: FunctionModule
date: 2019-06-24 18:03:31
```







# ���ܴ����



## ��ȡ cmd ִ�к���ı����

### Java
������Ѿ���������װ, ������ֲ�������������ʹ��, ֻ��Ҫ����һ���ַ������鼴��.</br>
```java
new cmdStrCommand(new String[]{"cmd","/C","type","C:\\Windows\\System32\\drivers\\etc\\hosts"}).ConsoleTerminalAscii();
```
���ܴ����:</br>
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



## ģ��ϵͳ�������Զ���¼����

### Java

���ô���:</br>
```java
new ProgramHead().getProgramHead();
```
���ܴ����:</br>
```java
public class ProgramHead {

    public static void getProgramHead(){

        System.out.println("\"I am Very Busy [�汾: 1.0.0_512]\"");
        System.out.println("(c) 2019-06-04 ����: StringOD. ��������Ȩ��");
        System.out.println();
        OutTime.setLongOutTime();

        OutTime.setLongOutTime();
        System.out.println("BIOS�Լ�..........................................���");
        OutTime.setLongOutTime();
        System.out.println("����Ӳ��...........................................26%");
        OutTime.setLongOutTime();
        System.out.println("����Ӳ��...........................................57%");
        OutTime.setLongOutTime();
        System.out.println("����Ӳ��...........................................���");
        OutTime.setLongOutTime();
        System.out.println("��ȡ�����ļ�........................................���");
        OutTime.setLongOutTime();
        System.out.println("����StringOD�ں�...................................���");
        OutTime.setLongOutTime();
        OutTime.setLongOutTime();
        System.out.println("����str����........................................���");
        OutTime.setLongOutTime();
        System.out.println("�����ں�ģ��........................................���");
        OutTime.setLongOutTime();
        OutTime.setLongOutTime();
        System.out.println("ִ��/Users/HiWin10/Desktop/TeLuoYiMuMa.exe.........���");
        OutTime.setLongOutTime();
        OutTime.setLongOutTime();
        System.out.println("����StrGUI.....���");
        OutTime.setLongOutTime();

        System.out.println("ִ���Զ���¼�ű�");
        OutTime.setShortOutTime();

        for (int i = 0; i < 10; i++)
            System.out.print("�z");
        System.out.println();
        String user = "�˻�: ";
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

        String password = "����: ";
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
            System.out.print("�z");
        System.out.println();

        System.out.println("��ӭ����\"I am Very Busy!\"");
        OutTime.setLongOutTime();
        System.out.println("��������");
        OutTime.setLongOutTime();

    }
}
```



## ���ļ�

### Java
```java
			//�򿪱��س����ļ���ʽ1
			Runtime rt = Runtime.getRuntime();
			String fileLac = "D:\\HBuilder\\HBuilder.exe";
	        rt.exec(fileLac);
		======================================
	        //�򿪱��س����ļ���ʽ2
		try {
	        Desktop desktop = Desktop.getDesktop();
	        File file = new File("C:\\Users\\HiWin10\\Desktop\\����֮·��������������.html");
	        desktop.open(file);
		}
		catch(IOException e) {
			System.out.println("�ļ����ܱ���");
		}
		======================================
	        �򿪱�����վ��Ĭ���������
		try {
	        URI uriNet = new URI("C:\\Users\\HiWin10\\Desktop\\����֮·��������������.html");
	        Desktop.getDesktop().browse(uriNet);
		}
		catch(URISyntaxException e) {
			System.out.println("URI��ַ����");
		}
		catch(IOException e) {
			System.out.println("�ļ����ܱ���");
		}
```



## ����Flash�ļ�

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



## ��Ӳ˵�

### Android
```java
public boolean onCreateOptionsMenu(Menu menu){
	getMenuInflater().inflate(R.menu.main,menu);
	//��ʾ�˵�
	return true;
}
```



## ��Ӳ˵���

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
	//��ʾ�˵���
	return true;
}
```

