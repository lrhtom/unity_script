1.事件函数执行机制
![Chromium 新标签页截图](.event_progess.png)
Time类
Time.deltaTime：每一帧的时间。
Time.fixedDeltaTime：固定帧率执行的时间。
Time.frameCount：运行帧的次数。
Time.time：框架运行的时间（秒）。
Time.realtimeSinceStartup：游戏开始后的实时时间。
### 1. **Time.deltaTime**
- **类型**：`float`
- **说明**：每一帧的时间（从上一帧到当前帧的时间间隔）。此值常用于确保游戏逻辑的时间依赖于帧率，而非固定值，常用于实现与帧率无关的平滑动画或运动。
  
  ```csharp
  float moveSpeed = 5f;
  transform.Translate(Vector3.forward * moveSpeed * Time.deltaTime);

  