# tbb_for_Images_Processing
记录自己使用tbb加速的一些图像处理的基础算法

VS2015 + OpenCV3.10    ------------   7672 x 7672 的图像;

01.RGB2Gray_tbb.cpp
循环100次： 
cvtColor(), 共耗时 51ms； 
RGB2Y(),共耗时 77ms; 使用tbb加速的RGB2Y(), 共耗时 22ms;
使用avx2的RGB2Y_6(),共耗时19ms, 使用 avx2+tbb的共耗时13.1ms;



02.RGB2YUV.cpp
yubtgfv


//
03.MedianBlur3X3
分辨率	算法优化	循环次数	速度
4032x3024	普通实现	100	8293.79ms
4032x3024	逻辑优化，更好的流水	100	83.75ms
4032x3024	SSE优化	100	11.93ms
4032x3024	AVX优化	100	9.32ms
