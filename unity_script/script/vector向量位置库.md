Vector2 a = new Vector2(2, 2);
print(a.magnitude);     //返回向量长度
print(a.sqrMagnitude);  //返回向量平方长度
print(a.normalized);    // 返回单位化的向量
a.Normalize();          //自身单位化

Vector2.Angle(a, b);    //返回a和b直接的角度
Vector2.ClampMagnitude(c, 2);   //返回长度小于2的矢量向量
Vector2.Distance(b, c);     //两个点之前的距离

// 同Mathf
Vector2.Lerp(a, b, 0.5f)；
Vector2.LerpUnclamped(a, b, 0.5f)；
Vector2.MoveTowards(a, target, Time.deltaTime);

//向量是结构体，是值类型，要整体赋值
transform.position = new Vector3(3, 3, 3);
Vector3 pos = transform.position;
pos.x = 10;
transform.position = pos;
