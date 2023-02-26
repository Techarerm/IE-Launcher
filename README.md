# IE-Launcher
在Windows 11上啟用Internet Explorer

>**警告**:如果你在乎安全性，別用。


Windows Defender會誤報，請關閉及時保護，安裝好在開啟。


更改啟動首頁:

1:打開C:\Program Files (x86)\Internet Explorer

2:右鍵ie.vbs編輯

3:貼上
```
With CreateObject("InternetExplorer.Application")
	.visible = True
	.Navigate "你想要的網址"
	.width = 800
	.height = 600
End With
```
記得更改，以下範例:
```
With CreateObject("InternetExplorer.Application")
	.visible = True
	.Navigate "http://www.google.com.tw"
	.width = 800
	.height = 600
End With
```
