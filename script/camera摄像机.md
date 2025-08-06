// 两种获取相机的方式
mainCamera = GameObject.Find("MainCamera").GetComponent<Camera>();
mainCamera = Camera.main; // tag必须为MainCamera

// 返回一个从相机到屏幕点的光线
Ray ray = mainCamera.ScreenPointToRay (Input.mousePosition);

// debug 画出射线
Debug.DrawRay (ray.origin, ray.direction * 10, Color.yellow);

// ray:射线对象
// layerMask:选择那个层进行碰撞检测
// hit:存放碰撞物体的信息
// maxDistance:最远距离
// 与那个层碰撞检测
RaycastHit hit; // 存放碰撞物体的信息
bool isCollider = Physics.Raycast (ray, out hit, 1000, LayerMask.GetMask ("MapCube"));
// 得到对象
MapCube mapCube = hit.collider.GetComponent<MapCube> ();
