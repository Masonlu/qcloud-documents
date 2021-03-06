

TKE 容器服务用户可以直接在控制台，通过配置日志收集规则进行集群内日志的收集，并将收集到的日志发送至日志服务 CLS 的指定日志主题。基于日志收集功能，使用日志服务平台可进行集群服务日志的实时检索、消费、投递等功能。

## 接入步骤

1. 登录 [容器服务控制台](https://console.cloud.tencent.com/tke2)，在左侧导航栏中，单击【日志采集】。在日志采集页面上方选择地域与集群后，单击【新建】。
2. 在新建日志收集规则页面，填写配置规则。
	 ![](https://main.qcloudimg.com/raw/1e5f4a44d4f1df9da059c726fe3b6ccb.png)
   配置解析如下：
<table>
   <tr>
      <th>配置项</th>
      <th>详情</th>
   </tr>
   <tr>
      <td>收集规则名称</td>
      <td>最长63个字符，只能包含小写字母、数字及分隔符("-")，且必须以小写字母开头，数字或小写字母结尾<br>配置名称设置后不可修改</td>
   </tr>
   <tr>
      <td>类型</td>
      <td>支持三种采集类型：采集容器标准输出日志、采集容器内文件日志、采集主机内文件日志
   </tr>
   <tr>
      <td>日志源</td>
      <td>可选择采集所有容器日志或指定的容器日志</td>
   </tr>
   <tr>
      <td>消费端</td>
      <td>选择日志服务 CLS</td>
   </tr>
   <tr>
      <td>日志服务实例</td>
      <td>选择日志集和日志主题；若现有的日志服务CLS不合适，您可以去控制台新建</td>
   </tr>
</table>
3. 单击【完成】，完成创建。
