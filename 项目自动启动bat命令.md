项目自动启动bat文件命令：

    @echo off
    set nodevars = "C:\Program Files\nodejs\nodevars.bat"
    
	     e:
	     cd work/system-back
	     cmd /k "%nodevars%npm rum dev"
       
    pause
 
