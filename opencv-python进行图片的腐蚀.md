## opencv实现图片的腐蚀
腐蚀操作关键是需要用到两个函数：一个是getStructuringElement（）,另一个是erode（）函数
相关解释如下：
getStructuringElement（内核的形状，大小），其中内核的形状位矩形、交叉形、椭圆形，大小以一对元组表示如（4，4）
erode（img1,kernel,iterations=1）,img1是原来的图片，kernel指腐蚀操作的内核，默认是一个简单的3X3矩阵，我们也可以利用getStructuringElement（）函数指明它的形状iterations指的是膨胀次数，省略是默认为1
## 实现代码

```groovy
import cv2 as cv
img=cv.imread('2.jpg',1)
## 开始进行腐蚀操作
img2=cv.getStructuringElement(cv.MORPH_CROSS,(10,10))##腐蚀预处理，确定处理核的大小,矩阵操作
img3=cv.erode(img,img2,iterations=1)#进行腐蚀操作
cv.imshow('origin',img)
cv.imshow('operation',img3)
cv.waitKey(0)
```
原图：
![在这里插入图片描述](https://img-blog.csdnimg.cn/2020120916400998.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2tpbmdKYW1lc2JvbmQ=,size_16,color_FFFFFF,t_70)
腐蚀之后：
![在这里插入图片描述](https://img-blog.csdnimg.cn/20201209164104784.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2tpbmdKYW1lc2JvbmQ=,size_16,color_FFFFFF,t_70)

