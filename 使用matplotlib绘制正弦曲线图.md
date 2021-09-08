### 我们都知道matplotlib是一个优秀的作图工具，那下面我们就用这个模块来画一下正弦曲线的图

```cpp
from matplotlib import pyplot as plt
import numpy as np
x=np.linspace(-3,3,100)#X的范围位于【-3，3】
y=np.sin(np.pi*x)
plt.title(r'$y=\sin(\pi\times x)$')#这是latex的表达式，与matlplotlib兼容
plt.plot(x,y,'ro')
#plt.plot(x, y, ls='-', lw=2, label='xxx', color='g' ) ls是线条的风格，lw是线条的宽度，label为标签文本
plt.show()#展示图象
```
![在这里插入图片描述](https://img-blog.csdnimg.cn/20201203125721308.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2tpbmdKYW1lc2JvbmQ=,size_16,color_FFFFFF,t_70)
![在这里插入图片描述](https://img-blog.csdnimg.cn/20201203130153989.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2tpbmdKYW1lc2JvbmQ=,size_16,color_FFFFFF,t_70)

