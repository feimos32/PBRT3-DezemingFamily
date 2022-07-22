# PBRT3-Dezeming Family

这是 [Dezeming Family : https://dezeming.top/] 的《PBRT3-零基础到精通系列》的随书源码。

开发环境：Visual Studio 2015及以上版本；Qt版本：5.5以上、6.0以下版本。注意除了VS2015，其他版本可能需要自行下载一些库的dll和lib文件，例如用于模型读写的assimp。

较大的模型文件请见网站：https://dezeming.top/?page_id=50 ； 注意：为了程序更简洁，并不检测模型文件是否存在。如果模型没有放到代码中定义的目录下，则可能会出现内存访问错误。

注：教程类代码不使用Git做版本控制管理，源码以压缩包格式给出。

后期发现的源码中的一些小Bug（等小Bug积累多了再统一修复更改）：

(1) PBRT系列15的源码中，透视投影相机的GenerateRayDifferential()和GenerateRay()函数没有加入：ray->medium = medium;



各个章节的软件界面：

<img src="https://github.com/feimos32/PBRT3-DezemingFamily/blob/main/Images/%E8%BD%AF%E4%BB%B6%E7%95%8C%E9%9D%A2-2-1.png" width="500px">

<img src="https://github.com/feimos32/PBRT3-DezemingFamily/blob/main/Images/%E8%BD%AF%E4%BB%B6%E7%95%8C%E9%9D%A2-3.png" width="500px">

<img src="https://github.com/feimos32/PBRT3-DezemingFamily/blob/main/Images/%E8%BD%AF%E4%BB%B6%E7%95%8C%E9%9D%A2-4.png" width="500px">

<img src="https://github.com/feimos32/PBRT3-DezemingFamily/blob/main/Images/%E8%BD%AF%E4%BB%B6%E7%95%8C%E9%9D%A2-5.png" width="500px">

<img src="https://github.com/feimos32/PBRT3-DezemingFamily/blob/main/Images/%E8%BD%AF%E4%BB%B6%E7%95%8C%E9%9D%A2-7.png" width="500px">

<img src="https://github.com/feimos32/PBRT3-DezemingFamily/blob/main/Images/%E8%BD%AF%E4%BB%B6%E7%95%8C%E9%9D%A2-8.png" width="500px">

<img src="https://github.com/feimos32/PBRT3-DezemingFamily/blob/main/Images/%E8%BD%AF%E4%BB%B6%E7%95%8C%E9%9D%A2-9.png" width="500px">

<img src="https://github.com/feimos32/PBRT3-DezemingFamily/blob/main/Images/%E8%BD%AF%E4%BB%B6%E7%95%8C%E9%9D%A2-9-1.png" width="500px">

<img src="https://github.com/feimos32/PBRT3-DezemingFamily/blob/main/Images/%E8%BD%AF%E4%BB%B6%E7%95%8C%E9%9D%A2-10.png" width="500px">

<img src="https://github.com/feimos32/PBRT3-DezemingFamily/blob/main/Images/%E8%BD%AF%E4%BB%B6%E7%95%8C%E9%9D%A2-11.png" width="500px">

<img src="https://github.com/feimos32/PBRT3-DezemingFamily/blob/main/Images/%E8%BD%AF%E4%BB%B6%E7%95%8C%E9%9D%A2-12-1.png" width="500px">

<img src="https://github.com/feimos32/PBRT3-DezemingFamily/blob/main/Images/%E8%BD%AF%E4%BB%B6%E7%95%8C%E9%9D%A2-12-2.png" width="500px">

<img src="https://github.com/feimos32/PBRT3-DezemingFamily/blob/main/Images/%E8%BD%AF%E4%BB%B6%E7%95%8C%E9%9D%A2-13.png" width="500px">

<img src="https://github.com/feimos32/PBRT3-DezemingFamily/blob/main/Images/%E8%BD%AF%E4%BB%B6%E7%95%8C%E9%9D%A2-14.png" width="500px">

<img src="https://github.com/feimos32/PBRT3-DezemingFamily/blob/main/Images/%E8%BD%AF%E4%BB%B6%E7%95%8C%E9%9D%A2-15-1.png" width="500px">

<img src="https://github.com/feimos32/PBRT3-DezemingFamily/blob/main/Images/%E8%BD%AF%E4%BB%B6%E7%95%8C%E9%9D%A2-15-2.png" width="500px">

<img src="https://github.com/feimos32/PBRT3-DezemingFamily/blob/main/Images/%E8%BD%AF%E4%BB%B6%E7%95%8C%E9%9D%A2-16.png" width="500px">

