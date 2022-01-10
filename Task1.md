# Matplotlib Learning 【Task 1】
## 使用matplotlib进行简单折线图的绘制
### Step 1: 载入工具包
- import matplotlib.pyplot as plt
- import matplotlib as mpl
- import numpy as np
### Step 2: 输入数据并绘制
- fig, ax = plt.subplots()
- ax.plot([1, 2, 3, 4], [1, 4, 3, 2])
![image](https://github.com/gluorokana/Dataanalysis/blob/master/Plot1.png)
### Step 3: 添加坐标轴和标题信息
- x = np.linspace(0, 2, 100)
- fig, ax = plt.subplots()  
- ax.plot(x, x, label='linear')  
- ax.plot(x, x**2, label='quadratic')  
- ax.plot(x, x**3, label='cubic')  
- ax.set_xlabel('x label') 
- ax.set_ylabel('y label') 
- ax.set_title("Simple Plot")  
- ax.legend() 
![image](https://github.com/gluorokana/Dataanalysis/blob/master/Plot2.png)
## 思考题
- OO模式简单易操作，但是难以应对同时有多图的情况。
