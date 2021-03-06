# GyroAllan

## 陀螺仪随机误差的Allan方差分析

陀螺仪的随机误差主要包括：量化噪声、角度随机游走、零偏不稳定性、角速率随机游走、速率斜坡和正弦分量。对于这些随机误差，利用常规的分析方法，例如计算样本 均值和方差，并不能揭示出潜在的误差源。另一方面，在实 际工作中通过对自相关函数和功率谱密度函数加以分析将随机误差分离出来是很困难的。Allan方差法是20世纪60年代由美国国家标准局的David Allan提出的，它是一种基于时域的分析方法。Allan方差法的主要特点是能非常容易地对各种误差源及其对整个噪声统计特性的贡献进行细致的表征和辨识，而且具有便于计算、易于分离等优点。 <br>

## 运行结果

![](https://github.com/XinLiGitHub/GyroAllan/raw/master/Software/untitled.bmp) <br>

量化噪声     X轴：0.458971 Y轴：0.564662 Z轴：1.118367  单位：urad <br>
角度随机游走  X轴：0.231291 Y轴：0.273737 Z轴：0.532305  单位：deg/h^0.5 <br>
零偏不稳定性  X轴：8.264598 Y轴：8.849770 Z轴：7.367757  单位：deg/h <br>
角速率游走   X轴：42.156012 Y轴：40.870664 Z轴：32.268721  单位：deg/h/h^0.5 <br>
速率斜坡     X轴：43.040958 Y轴：40.022454 Z轴：11.171091  单位：deg/h/h <br>

## 注意

当Allan标准差的拟合多项式中的拟合系数是负值时，所得误差项的拟合结果随着相关时间的微小改变变化很大，拟合误差很大，可信度差。
