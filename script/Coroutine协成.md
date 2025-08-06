private IEnumerator ie;
ie = Fade();
// 第一种
StartCoroutine(ie);       // 启动
StopCoroutine(ie);        // 关闭
// 第二种
StartCoroutine("Fade");   // 启动
StopCoroutine("Fade");    // 关闭

IEnumerator Fade()
{
  while (true)
  {
      // do something
      yield return new WaitForSeconds(2);   // 返回值必须是yield这种形式
  }
}
