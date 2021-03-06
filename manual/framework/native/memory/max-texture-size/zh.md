# 各平台硬件所允许的最大纹理尺寸 #

按道理来说，cocos2d-x是可以显示任何大小纹理，但是实际上纹理大小由于硬件和操作系统原因是有限制的。 

这里我们提供一个不同平台模拟器上纹理大小限制的表格 

|platform | maxsize in pixels|
|----------- | -----------|
|win32 | `2048*2048`  |
|android |  `4096*4096` | 
|iphone3 | `1024*1024`  |
|iphone3gs | `2048*2048`  |
|iphone4 | 2048*2048  |

在真实的机器上面，也有一些不同的限制，这里有一些测试结果：G3 `1024*1024, iPhone4 2048*2048` 

因此对于开发者来说，假如你想要跨平台，并且游戏运行流畅，你最好保持你的纹理大小小于1024*1024，这个是大多数机器的限制。
