## 性能调优

讨论到iOS性能基本会让人想起的就是CPU和GPU，那我们需要在这两个方面优化的方向都有哪些呢？

### CPU

- 帧率：保持60 FPS
- 不必要的CPU渲染：可以把一些渲染放到GPU中去
- 更多的屏外渲染：最好没有
- 更多的混合：更少
- 任何奇怪的图片格式或大小：避免动态调整和转换图片

### GPU

- 帧率：保持60 FPS
- CPU、GPU限制：较低的利用率和保持电量
- 不必要的CPU渲染：可以把一些渲染任务放到GPU中

### View Debuging

- 避免任何昂贵的views or effects
- 避免混乱的视图层次结构

![Core Animation Pipeline](https://github.com/JerryNil/iOSNotes/blob/master/iOS%E5%B0%8F%E6%8A%84%EF%BC%9AAnimation%20and%20%E6%80%A7%E8%83%BD%E4%BC%98%E5%8C%96/CoreAnimationPipeline.jpg)
