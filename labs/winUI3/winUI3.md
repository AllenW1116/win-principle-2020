# Get started with WinUI 3 for desktop apps

<https://docs.microsoft.com/en-us/windows/apps/winui/winui3/get-started-winui3-for-desktop>

***

<https://github.com/principleWindows/WinUI-3-Demos>



## 1 Configure your dev environment


### 1.1 Install Visual Studio 2019 Preview


���� winUI 3.0 ������ Release Candidate ״̬, ������ Visual Studio 2019 Community ��������ʽ֧��,
Ϊ����������Ҫ��װ Visual Studio 2019 Preview �� Community �汾���ٷ����ص�ַ��
<https://visualstudio.microsoft.com/vs/preview/>

You must include the following workloads when installing the Visual Studio Preview:
* .NET Desktop Development
* Universal Windows Platform development
 
To build C++ apps you must also include the following workloads:
* Desktop development with C++
* The C++ (v142) Universal Windows Platform tools optional component for the Universal Windows Platform workload

![optional component](pix/installVSPreview.PNG)


��ס��װʱҪѡ��Ӣ�����԰�, ���� Visual Studio 2019 Preview �Ļ�������ΪӢ�

![optional component](pix/installen.png)

��װ����������Ժ����� Visual Studio 2019 Preview ��ѡ�� **�������������** ����VS �����档

![optional component](pix/startPreview.png)

ѡ�� **����** -> **ѡ��** ����ѡ����档

![optional component](pix/setlanguage1.png)

ѡ�� **����** -> **��������** -> **����** -> **Engligh** ȷ�������� VS��

ע�⣺��Ҫ�� **Visual Studio Installer** �а�װ��Ӣ�����԰�����Ż��� **English** ѡ����֮ǰû�а�װ���Խ��� **Visual Studio Installer** �� **Visual Studio 2019 Preview** �����޸ġ�

![optional component](pix/setlanguage2.png)

������ʾ�ľ���Ӣ�Ľ�������

![optional component](pix/englishUI.png)


### 1.2 Install .NET 5 Release Candidate
Install both x64 and x86 versions of .NET 5 rc:

<https://dotnet.microsoft.com/download/dotnet/5.0>

### 1.3 Install WinUI 3 Preview 1 Visual Studio project templates

�� Visual Studio 2019 Preview Community, �� Extensions �� Online ������ 
WinUI 3 Project Templates���ҵ���װ�ò����
**�������İ�װ�ǳ����������������ذ�װ��Ȼ�ܿ���ʧ�ܡ�**

Ҳ����ֱ��ȥ<https://marketplace.visualstudio.com/items?itemName=Microsoft-WinUI.WinUIProjectTemplates>
���ذ�װ��

## 2 Create a WinUI 3 desktop app for C++/Win32

<https://docs.microsoft.com/en-us/windows/apps/winui/winui3/get-started-winui3-for-desktop#create-a-winui-3-desktop-app-for-cwin32>

1. In Visual Studio 2019, select File -> New -> Project.

2. In the project drop-down filters, select C++, Windows, and WinUI.

3. Select the Blank App, Packaged (WinUI in Desktop) project type and click Next.

![new project](pix/newProj.PNG)

4. Enter a project name, choose any other options as desired, and click Create.

5. In the following dialog box, set the Target version to Windows 10, 
version 2004 (build 19041) and Minimum version to Windows 10, version 1809 
(build 17763) and then click OK.

![project platform](pix/projectPlatform.PNG)

6. At this point, Visual Studio generates two projects:

* Project name (Desktop): This project contains your app's code. The App.xaml and 
various App code files define an Application class that represents your app instance, 
and the MainWindow.xaml and various MainWindow code files define a MainWindow class 
that represents the main window displayed by your app. These classes derive from 
types in the Microsoft.UI.Xaml namespace provided by WinUI.

![App Project](pix/app.PNG)

* Project name (Package): This is a Windows Application Packaging Project that is 
configured to build the app into an MSIX package. This provides a modern deployment 
experience, the ability to integrate with Windows 10 features via package extensions, 
and much more. This project contains the package manifest for your app, and it is the 
startup project for your solution by default.

![Package Project](pix/packManifest.PNG)

7. To add a new item to your app project, right-click the Project name (Desktop) project 
node in Solution Explorer and select Add -> New Item. In the Add New Item dialog box, 
select the WinUI tab, choose the item you want to add, and then click Add. For more 
details about the available items, see [this section](https://docs.microsoft.com/en-us/windows/apps/winui/winui3/#item-templates-for-winui-3).

![New Item](pix/newItem.PNG)

8. Build and run your solution to confirm that the app runs without errors.


