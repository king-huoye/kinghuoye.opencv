## 实现图像模糊
关键函数blur(img,size):需要处理的图像，后面的参数为处理的尺寸,size同前面的腐蚀处理一样都是一个n*m的格式

```cpp
import cv2 as cv
img1=cv.imread('5b90f4871daba (1).jpg',1)
cv.imshow('origin',img1)
img2=cv.blur(img1,(3,7))#需要处理的图像，后面的参数为处理的尺寸
cv.imshow('blur',img2)
cv.waitKey(0)
```
## 原图
![在这里插入图片描述](https://img-blog.csdnimg.cn/20201209170152128.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2tpbmdKYW1lc2JvbmQ=,size_16,color_FFFFFF,t_70)
## 模糊之后
![在这里插入图片描述](https://img-blog.csdnimg.cn/20201209170208145.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2tpbmdKYW1lc2JvbmQ=,size_16,color_FFFFFF,t_70)
