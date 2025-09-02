// 设置物体旋转的两种方式：
cube.eulerAngles = new Vector3(45, 45, 45);
cube.rotation = Quaternion.Euler(new Vector3(45, 45, 45));

// 应用场景，玩家平滑旋转面向敌人
Vector3 dir = enemy.position - player.position;
dir.y = 0;    //取消在y轴（上下）方向的旋转
Quaternion target= Quaternion.LookRotation(dir);
player.rotation = Quaternion.Lerp(player.rotation, target, Time.deltaTime);
