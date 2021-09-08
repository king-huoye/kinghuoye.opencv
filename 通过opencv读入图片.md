```python
import cv2 as cv
img=cv.imread('0110aa5dcf95b5a8012053c002fe99.jpg@1280w_1l_2o_100sh.jpg')
cv.imshow('mypicture',img)
cv.waitKey(0)
```
## 相关要求
使用前需要导入CV2这个模块
imread（）函数表示读取照片，括号里面的参数放图片的路径
imshow():第一个参数表示显示图片窗口的名称，第二个参数表示储存图片数据的名称
waitkey()表示键盘绑定参数，当key为0，需要指出的是它的时间尺度是毫
秒级。函数等待特定的几毫秒，看是否有键盘输入。
