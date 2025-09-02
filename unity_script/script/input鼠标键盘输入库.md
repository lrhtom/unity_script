// 鼠标按键
Input.GetMouseButton();     //鼠标按下触发
Input.GetMouseButtonDown(); //鼠标按下不动持续触发
Input.GetMouseButtonUp();   //鼠标松开触发

// 键盘按键，同理
Input.GetKey();
Input.GetKeyDown();
Input.GetKeyUp();

//Unity中设置的虚拟按键
Input.GetButton();
Input.GetButtonDown();
Input.GetButtonUp();

// 返回由axisName标识的虚拟轴的值
Input.GetAxis("Horizontal") //平滑的获取水平方向按键的值 [-1, 1]： A D ← →
Input.GetAxisRaw("Horizontal")//平滑的获取水平方向按键的值- 1 0 1： A D ← →
// 同理垂直方向
Input.GetAxis("Vertical")   // W S ↑ ↓


// 静态属性，任何键（鼠标或者键盘）
Input.anyKeyDown;
Input.anyKey;

Input.mousePosition；    // 获取鼠标的相对于untiy的坐标，左下为(0,0)
