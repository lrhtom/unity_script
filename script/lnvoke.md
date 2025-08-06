相当于定时调用函数
Invoke("Attack",3);       //3秒后调用Attch方法
InvokeRepeating("Attack", 4, 2);  //4秒后每隔2秒调用一次Attach
CancelInvoke("Attack");       // 取消调用Attach定时器
bool res = IsInvoking("Attack");  //判断Attach定时器是否还存在
