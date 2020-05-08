# tbb_for_Images_Processing
记录自己使用tbb加速的一些图像处理的基础算法

VS2015 + OpenCV3.10

01.RGB2Gray_tbb.cpp
处理一张7672 x 7672 的图像,循环100次： 
cvtColor(), 共耗时 51ms； 
RGB2Y(),共耗时 77ms; 使用tbb加速的RGB2Y(), 共耗时 22ms;
使用avx2的RGB2Y_6(),共耗时19ms, 使用 avx2+tbb的共耗时13.1ms;



02.RGB2YUV.cpp
