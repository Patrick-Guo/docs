---
---

# **创建并定义产品**

本文将以RGB灯产品举例，快速体验产品创建流程。

## **创建产品**

登录账号后在产品开发-&gt;产品管理页面点击创建产品按钮。

第一步：选择品类。通过品类搜索RGB灯快速选中，或在标准品类列表中找到电工照明一级品类下的RGB灯。

第二步：选择方案。您可选择系统中已预设的推荐方案完成快速创建，也可以通过自定义方案根据实际需要进行配置，此处我们以自定义方案进行配置。



第三步：选择产品的联网类型与通讯方式。此处我们选择单品设备类型、2G/3G/4G/5G联网方式、数据格式使用物模型类型。







第四步：最后上传产品图片、输入产品名称，提交并完成产品创建。



创建成功后平台将为该产品分配ProductKey与ProductSecret，用于后续设备需连接平台时的鉴权。



## **功能定义**

产品创建后可进入产品详情的功能定义页面进行物模型功能定义。

以RGB灯的功能举例，点击物模型编辑并添加以下功能点：

<table style="">
<tr>
<p><strong>功能ID</strong></p>
<p><strong>功能类型</strong></p>
<p><strong>功能名称</strong></p>
<p><strong>标识符</strong></p>
<p><strong>数据类型</strong></p>
<p><strong>数据定义</strong></p>
<p><strong>读写类型</strong></p>
<p><strong>备注</strong></p>
</tr>
<tr>
<td><p>1</p></td>
<td><p>属性</p></td>
<td><p>开关</p></td>
<td><p>Switch</p></td>
<td><p>Bool</p></td>
<td><p>False：关灯True：开灯</p></td>
<td><p>读写</p></td>
<td><p /></td>
</tr>
<tr>
<td><p>2</p></td>
<td><p>属性</p></td>
<td><p>颜色R</p></td>
<td><p>Red</p></td>
<td><p>INT</p></td>
<td><p>最小值：0最大值：255</p></td>
<td><p>读写</p></td>
<td><p>红色灯色值，用于组成彩灯颜色</p></td>
</tr>
<tr>
<td><p>3</p></td>
<td><p>属性</p></td>
<td><p>颜色G</p></td>
<td><p>Green</p></td>
<td><p>INT</p></td>
<td><p>最小值：0最大值：255</p></td>
<td><p>读写</p></td>
<td><p>绿色灯色值，用于组成彩灯颜色</p></td>
</tr>
<tr>
<td><p>4</p></td>
<td><p>属性</p></td>
<td><p>颜色B</p></td>
<td><p>Blue</p></td>
<td><p>INT</p></td>
<td><p>最小值：0最大值：255</p></td>
<td><p>读写</p></td>
<td><p>蓝色灯色值，用于组成彩灯颜色</p></td>
</tr>
<tr>
<td><p>5</p></td>
<td><p>属性</p></td>
<td><p>亮度</p></td>
<td><p>Brightness</p></td>
<td><p>INT</p></td>
<td><p>最小值：0最大值：100</p></td>
<td><p>读写</p></td>
<td><p>用于控制灯光亮度大小</p></td>
</tr>
<tr>
<td><p>6</p></td>
<td><p>属性</p></td>
<td><p>延时关灯时间</p></td>
<td><p>Delay</p></td>
<td><p>INT</p></td>
<td><p>最小值：0最大值：86400</p></td>
<td><p>读写</p></td>
<td><p>用于设置倒计时关灯时间</p></td>
</tr>
</table>

创建完成后点击发布应用生效物模型，发布成功后，平台将为每个属性分配功能ID。后续设备与平台将通过该ID进行

数据交互。