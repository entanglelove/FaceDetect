# 如何在Windows安裝OpenCV Python設定
How Install OpenCV in  on Windows for Python

## 安裝  numpy
先下載numpy <br>
到 [numpy](https://pypi.python.org/pypi/numpy)  <br>
下載對應的NumPy版本 <br>
我在這裡是下載 numpy-1.11.0-cp27-none-win_amd64.whl (64位元)<br>
接著使用cmd (命令提示字元) 輸入<br>
```
pip install numpy-1.11.0-cp27-none-win_amd64.whl
```
如果沒出現錯誤訊息，則會正常安裝<br>
可再用下面指令檢查是否安裝成功<br>
使用IDLE (Python GUI) 輸入<br>
```
import numpy
numpy.__version__
```
如安裝成功，則會顯示安裝的版本<br>
'1.11.0'<br>
如下圖<br>
![alt tag](http://i.imgur.com/77S8vj2.jpg)

## 如何安裝OpenCV
下載OpenCV <br>
到官網下載[OpenCV](http://opencv.org/downloads.html) <br>
我在這裡下載的版本是 OpenCV 2.4.12 Windows Pre-built <br>
將OpenCV解壓縮到任一地方，例如C:\，解壓後會多出一個名稱為opencv的資料夾 <br>
再到opencv資料夾搜尋<b> cv2.pyd </b>，尋找自己對應的的位元 <br>
<b> cv2.pyd </b>的資料夾路徑為 <br>
C:\opencv\build\python\2.7\x86  (32位元) <br>
C:\opencv\build\python\2.7\x64  (64位元) <br>
將<b> cv2.pyd </b>複製到 C:\Python27\Lib\site-packages 路徑下<br>
可再用下面指令檢查是否安裝成功 <br>
使用IDLE (Python GUI) 輸入<br>
```
import cv2
print cv2.__version__
```
如安裝成功，則會顯示安裝的版本<br>
'2.4.12'<br>
如下圖<br>
![alt tag](http://i.imgur.com/Njp1IUk.jpg)

## Environment
* Windows 8.1
* Python 2.7.3
* OpenCV 2.4.12 
* numpy 1.11.0
