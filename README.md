# Oraco-system
like Linux（Android）

    简介：Oraco系统是一个基于C++编写的原生命令行操作系统。它模拟了Linux的一些基本功能，如文件操作、进程管理等。本教程将详细介绍如何使用Oraco系统，包括如何安装和运行程序，以及如何使用各种内置命令。
 2. 安装和运行程序

2.1 下载Oraco系统源代码

首先，从GitHub上下载Oraco系统的源代码：https://github.com/OracoSystem/OracoSystem

2.2 编译Oraco系统

解压下载的源代码包，然后在源代码目录下打开终端。执行以下命令来编译Oraco系统：

bash
g++ -o oraco system.cpp


这将生成一个名为`oraco`的可执行文件。

2.3 运行Oraco系统

在终端中输入以下命令来运行Oraco系统：

bash
./oraco

这将启动Oraco系统的命令行界面。

3. 使用内置命令

Oraco系统提供了许多内置命令，以下是一些常用的命令及其用法：

3.1 cd <home>

切换到指定的目录。例如，要切换到`/home`目录，可以输入：
>>cd /home

 3.2 `ls`

列出当前目录下的文件和子目录。例如：

```
>>ls
file1.txt file2.txt
```

3.3 `pwd`

显示当前工作目录的路径。例如：

```
>>pwd
/home
```

3.4 `exit`

退出Oraco系统。例如：

```
>>exit
```

3.5 `mkdir new_folder`

创建一个新目录。例如：

>>mkdir new_folder

3.6 `rm new_folder`

删除一个目录。例如：

>>rm new_folder

3.7 `cd file1.txt file2.txt`

将`file1.txt`和`file2.txt`两个文件合并为一个新的文件。例如：

```
>>cd file1.txt file2.txt
>>file1.txt copied to file2.txt.
```

### 3.8 `mv file1.txt file2.txt`

将`file1.txt`重命名为`file2.txt`。例如：

```
>>mv file1.txt file2.txt
```

### 3.9 `cat file1.txt`

显示`file1.txt`文件的内容。例如：

```
>>cat file1.txt
Hello, World!
```

### 3.10 `echo 'Hello, World!'`

输出字符串`Hello, World!`。例如：

```
>>echo 'Hello, World!'
Hello, World!
```

### 3.11 `date`

显示当前的日期和时间。例如：

```
>>date
2022-01-01 12:00:00
```

### 3.12 `cal`

显示日历。例如：

```
>>cal
    January 2022
Mo Tu We Th Fr Sa Su
                  1
 2  3  4  5  6  7  8
 9 10 11 12 13 14 15
16 17 18 19 20 21 22
23 24 25 26 27 28 29
30 31
```

### 3.13 `man ls`

显示`ls`命令的帮助信息。例如：

```
>>man ls
NAME
    ls - list directory contents
SYNOPSIS
    ls [OPTION]... [FILE]...
DESCRIPTION
    List directory contents. With the -l option, do not list symbolic links, but list the target of each symbolic link. The -a option do not ignore entries starting with . and do not list implied . and ..
```

### 3.14 `web`

访问指定的网站。例如，要访问www.google.com，可以输入：

```
>>web www.google.com
```

### 3.15 `root`

以超级用户权限运行命令。例如，要以超级用户权限运行`ls`命令，可以输入：

```
>>root ls
```

### 3.16 `adb devices`

列出已连接的设备。例如：

```
>>adb devices
List of devices attached
emulator-5554     device
```

### 3.17 `adb shell`

进入设备的shell环境。例如：

```
>>adb shell
$ adb devices
List of devices attached
emulator-5554     device
$ adb shell getprop ro.product.model
Pixel 4a (API 28)
```

### 3.18 `reboot`

重启设备。例如：

```
>>reboot
```

### 3.19 `update`

更新Oraco系统。例如：

```
>>update
Updating Oraco System...
Update completed. Rebooting...
```

### 3.20 `install app`

安装应用程序。例如，要安装一个名为`app1`的应用程序，可以输入：

```
>>install app app1
Installing app1...
Installation completed.
```

### 3.21 `uninstall app`

卸载应用程序。例如，要卸载一个名为`app1`的应用程序，可以输入：

```
>>uninstall app app1
Uninstalling app1...
Uninstallation completed.
```

### 3.22 `run app`

运行应用程序。例如，要运行一个名为`app1`的应用程序，可以输入：

```
>>run app app1
Running app1...
App1 started successfully.
```

### 3.23 `stop app`

停止应用程序。例如，要停止一个名为`app1`的应用程序，可以输入：

```
>>stop app app1
Stopping app1...
App1 stopped successfully.
```

### 3.24 `send message`

发送短信。例如，要给电话号码为`1234567890`的用户发送一条短信内容为`Hello, World!`，可以输入：

```
>>send message 1234567890 Hello, World!
Sending message...
Message sent successfully.
```

### 3.25 `call`

拨打电话。例如，要给电话号码为`1234567890`的用户打电话，可以输入：

```
>>call 1234567890
Dialing...
Call connected.
```

### 3.26 `record video`

录制视频。例如，要录制一段时长为10秒的视频，可以输入：

```
>>record video 10s
Recording video...
Video recorded successfully. Saved as video1.mp4.
```

### 3.27 `stop recording`

停止录制视频。例如，要停止录制视频，可以输入：

```
>>stop recording video1.mp4
Stopping recording... Video saved as video1.mp4.
```

### 3.28 `play video`

播放视频。例如，要播放名为`video1.mp4`的视频，可以输入：

>>play video video1.mp4
Playing video... Video playback completed.
