//静态属性
Mathf.Deg2Rad;  //角度转弧度
Mathf.Rad2Deg;  //弧度转角度
Mathf.Infinity; //正无穷的数
Mathf.NegativeInfinity； //负无穷的数
Mathf.Epsilon;  //最小的浮点正数

// 静态方法
Mathf.Floor();  //向下取整，返回浮点数
Mathf.FloorToInt(); //向下取整，返回正整数
Mathf.ClosestPowerOfTwo(30);    //返回2^N最接近30的数，这里就是8.
Mathf.Clamp(Time.time, 1.0F, 3.0F)  //Time.time<1返回1，大于3返回3，中间返回自身
Mathf.Lerp(a, b, t） //差值运算，返回 a+(b-a)*t 其中t=Mathf.Clamp(t,0,1)
Mathf.LerpUnclamped(a, b, t）    //差值运算，返回 a+(b-a)*t，t不做限制可以小于0，大于1
Mathf.MoveTowards(x, 10, Time.deltaTime*speed)  //从x变化到10，以每秒spped的速度
Mathf.PingPong(t, 20)   //返回的值将在0到20直接来回移动，比如0到20到0到20，t=19返回19 t=21返回19 t=40返回0


Random.InitState();：随机种子，种子相同随机出来的数的顺序也相同 
(int)System.DateTime.Now.Ticks 想要不相同可以传入时间。
Random.Range(4, 100)：随机返回[4, 99]中的一个整数
Random.Range(4, 5f)：随机返回[4.0, 5.0]中的一个浮点数
