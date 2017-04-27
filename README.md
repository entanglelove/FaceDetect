# FaceDetect
臉部偵測 for Windows use Python 
Python OpenCV Tutorial

* [Demo Video]() - Windows - update  
* [Demo Video](https://youtu.be/TnnSfnjw6js) - Windows 

## 特色
* 圖片、影片 臉部偵測

## 建立環境

Python 3.5.2 + OpenCV 3.1.0   (建議用這個，更簡單)
請參考[]()

Python 2.7.3 + OpenCV 2.4.12
請先確定電腦上已經安裝<b> OpenCV </b>和<b> numpy </b><br>
可參考[如何在Windows安裝OpenCV Python設定](https://github.com/twtrubiks/FaceDetect/tree/master/How%20Install%20OpenCV%20in%20on%20Windows%20for%20Python)<br>

## 如何使用

Python 3.5.2 + OpenCV 3.1.0
```
python face_detect_python3.py
```


Python 2.7.3 + OpenCV 2.4.12
```
python face_detect_python2.py [圖片檔名] [haarcascade.xml]
```

## 執行範例

Python 3.5.2 + OpenCV 3.1.0
```
python face_detect_python3.py
```


Python 2.7.3 + OpenCV 2.4.12
```
python face_detect_python2.py
```

## 執行過程
程式執行後，會自行跳出偵測臉部的圖片<br>
![alt tag](http://i.imgur.com/u8m9lUf.jpg)

## 輸出
目錄底下會多出一張名稱為 face_detection.jpg 的圖片 <br>
![alt tag](http://i.imgur.com/evl398U.jpg)

## 備註
程式基本上只做了小小的修改，<br>
我發現<b> haarcascade_frontalface_alt.xml </b>比原作者的<b> haarcascade_frontalface_default.xml </b>有更好的辨識率，<br>
更多的<b> haarcascade </b>可到<b> opencv </b>路徑裡<b> opencv\sources\data\haarcascades </b>取得，<br>
路徑底下還有<b> haarcascade_eye.xml </b>偵測眼睛之類的，大家可以自行摸索，<br>
最後，請注意，這是<b> 臉部偵測 </b>，並不是 <b> 臉部辨識 </b>

## 其他
更多的資訊可參考原作者<br>

Run the code like this:

*python face_detect.py abba.png haarcascade_frontalface_default.xml*

If you want to understand how the code works, the details are here:

https://realpython.com/blog/python/face-recognition-with-python/

## 後記 

本篇文章所介紹的是 **臉部偵測 ( Face Detection )**，並不是 **臉部辨識 ( Face Recognize)**

因為小弟有稍微研究一點***臉部辨識 ( Face Recognize)**，所以順便來分享我的心得

如果要辦到***臉部辨識 ( Face Recognize)**，OpenCV 其實也可以辦到，可以透過OpenCV官網提供的演算法來完成，OpenCV官方有提供三種Face Recognition演算法，
分別為 EigenFaceRecognizer、FisherFaceRecognizer、 LBPHFaceRecognizer。

最後我選擇 LBPHFaceRecognizer，為什麼不選 EigenFaceRecognizer 或 FisherFaceRecognizer 呢?

因為 LBPHFaceRecognizer 有幾個優點：
1. 訓練和比對的圖片大小可以不一致。
2. 比較不會受到光線以及角度的影響 ( 辨識率 )。
3. 可以直接更新訓練資料庫，不用全部重新訓練。

流程大致上是
收集人臉 --> 訓練  --> 得到一個 dataSet 
然後透過這個 dataSet  下去辨識。

我認為使用 OpenCV 提供的Face Recognition演算法效果沒有非常好，或許可以考慮用目前最紅的深度學習 (Deep learning) 處理精準度的問題。
 



## 執行環境
* Windows 8.1
* Python 2.7.3
* OpenCV 2.4.12 
* numpy 1.11.0

## License
MIT license
