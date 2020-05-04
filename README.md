# tbb_for_Images_Processing
使用tbb加速的一些图像处理的基础算法

01.RGB2Gray_tbb.cpp
处理一张7672 x 7672 的图像,循环100次： cvtColor(), 共耗时 51ms； RGB2Y(),共耗时 77ms; 使用tbb加速的RGB2Y(), 共耗时 22ms.
