# Agile——运动场馆预约助手
|文档名称|Agile——运动场馆预约助手项目文档|
|----|:----|
|产品名称|Agile|
|产品描述|一款可以预定几乎所有运动类型场馆、指引用户租购运动装备的APP|
|产品版本|1.0|
|文档作者|汪铭宇|
## 项目说明
### 价值宣言
Agile——运动场馆预约助手，是一款通过调用全国运动场馆位置数据，向用户智能推荐运动场馆并支持线上预定场地的app。用户可通过Agile快速了解场馆信息后快速预定场地；还可使用指引功能租借运动装备、购买运动补给，获得更好的运动体验；还可通过组队功能发起组队。Agile，让运动更方便。
### Agile核心功能结构图
![产品核心功能结构图](https://github.com/miyukiwg/API-final-project/blob/main/img/%E6%A0%B8%E5%BF%83%E5%8A%9F%E8%83%BD%E7%BB%93%E6%9E%84%E5%9B%BE.png)
### 项目简述
本项目通过对运动场馆预约类APP用户的需求分析，再结合课程所学的编程、API知识和其他课程知识，设计出满足用户需求、缓释用户痛点的解决方案。
## 一、用户需求分析
### （一）背景介绍与用户画像
#### 1、背景介绍
如今，使用手机预定酒店、出行车票已十分常见。但在运动场馆预约这方面，缺少能够整合各运动类型场馆的预定APP。用户想要寻找运动场馆时往往要通过比较复杂的步骤、或是为了预定场地在各个APP中切换；且市场上常见的运动场地预定类APP能预约的运动场馆类型比较单一。因此，用户快速预定场地、得知场馆信息、租借器材等需求有待满足。
#### 2、用户画像
![用户画像](https://github.com/miyukiwg/API-final-project/blob/main/img/%E7%94%A8%E6%88%B7%E7%94%BB%E5%83%8F.png)
### （二）价值主张画布
根据对用户的需求分析、多款运动场地预定类APP的使用体验和通过对经常运动的朋友们的调查。我列出了以下价值主张画布：
![价值主张画布](https://github.com/miyukiwg/API-final-project/blob/main/img/%E4%BB%B7%E5%80%BC%E4%B8%BB%E5%BC%A0%E7%94%BB%E5%B8%83.png)
### （三）用户旅程图
在通过以上的分析，我绘制了Agile的用户旅程图，帮助进一步理解用户在使用场地预约类APP时的目标、需求和感受，并列出痛点及对应的解决方案。
![用户旅程图](https://github.com/miyukiwg/API-final-project/blob/main/img/%E7%94%A8%E6%88%B7%E6%97%85%E7%A8%8B%E5%9C%B0%E5%9B%BE.png)

以下的解决方案将描述本产品是如何运用本课程所学的编程、API知识把用户需求与产品价值契合。

## 二、解决方案
本项目的整体规划图如下
此处应有规划图
### （一）设计
根据价值主张结合用户需求，分别绘制了Agile的功能结构图、信息结构图、产品结构图，以及预定业务的流程图。
#### 1、功能结构图
![功能结构图](https://github.com/miyukiwg/API-final-project/blob/main/img/功能结构图.png)
#### 2、信息结构图
#### 3、产品结构图
#### 4、预定业务流程图
### （二）创建
#### 1、功能列表
结合价值主张画布和以上结构图、流程图列出的Agile功能列表：

<table>
   <tr>
      <td>用户界面模块</td>
      <td>功能</td>
      <td>子功能</td>
      <td>功能描述</td>
   </tr>
   <tr>
      <td rowspan="6" style="text-align:center;">首页</td>
      <td style="text-align:center;">Flash广告</td>
      <td></td>
      <td>显示最近的热点新闻</td>
   </tr>
   <tr>
      <td style="text-align:center;">地区选择</td>
      <td></td>
      <td>根据用户所在地区推荐附近场馆</td>
   </tr>
   <tr>
      <td style="text-align:center;">场馆搜索</td>
      <td></td>
      <td>可根据输入的关键词进行搜索，并列出结果</td>
   </tr>
   <tr>
      <td style="text-align:center;">场馆分类</td>
      <td></td>
      <td>对APP内可预定的运动场地类型进行划分，方便用户查找</td>
   </tr>
   <tr>
      <td style="text-align:center;">订单提醒</td>
      <td></td>
      <td>提醒用户按时到达预定场地参加运动</td>
   </tr>
   <tr>
      <td style="text-align:center;">场馆推荐</td>
      <td></td>
      <td>根据智能算法向用户推荐运动场馆</td>
   </tr>
   <tr>
      <td rowspan="9" style="text-align:center;">发现页</td>
      <td rowspan="2" style="text-align:center;">指引</td>
      <td style="text-align:center;">租借</td>
      <td>根据用户坐标向用户推荐附近可租借运动装备的店铺</td>
   </tr>
   <tr>
      <td style="text-align:center;">购买</td>
      <td>根据用户坐标向用户推荐附近可购买运动装备、补给的店铺</td>
   </tr>
   <tr>
      <td rowspan="3" style="text-align:center;">组队</td>
      <td style="text-align:center;">参与</td>
      <td>若符合条件，用户可参与由他人发起的组队</td>
   </tr>
   <tr>
      <td style="text-align:center;">发起</td>
      <td>用户可以个人名义发起运动组队</td>
   </tr>
   <tr>
      <td style="text-align:center;">讨论</td>
      <td>用户可在组队页面下进行讨论</td>
   </tr>
   <tr>
      <td rowspan="4" style="text-align:center;">私信</td>
      <td style="text-align:center;">系统信息</td>
      <td>提醒用户APP的更新、优化或其他信息</td>
   </tr>
   <tr>
      <td style="text-align:center;">订单信息</td>
      <td>显示用户订单状态、告知用户预定成功</td>
   </tr>
   <tr>
      <td style="text-align:center;">组队信息</td>
      <td>显示用户参与或发起组队的信息</td>
   </tr>
   <tr>
      <td style="text-align:center;">显示用户私信</td>
      <td>显示用户收到其他人的私信</td>
   </tr>
   <tr>
      <td rowspan="10" style="text-align:center;">我的</td>
      <td style="text-align:center;">用户信息</td>
      <td></td>
      <td>用户可自行修改用户信息，并显示粉丝、关注数</td>
   </tr>
   <tr>
      <td style="text-align:center;">记录运动时长</td>
      <td></td>
      <td>根据用户订单的运动时间，显示用户的运动时长</td>
   </tr>
   <tr>
      <td style="text-align:center;">记录打卡场馆</td>
      <td></td>
      <td>根据用户订单的运动场馆，显示用户成功消费的场馆</td>
   </tr>
   <tr>
      <td rowspan="3" style="text-align:center;">订单信息</td>
      <td style="text-align:center;">支付</td>
      <td>用户可支付之前下单但未支付的订单</td>
   </tr>
   <tr>
      <td style="text-align:center;">完成</td>
      <td>用于用户提前完成订单</td>
   </tr>
   <tr>
      <td style="text-align:center;">退款</td>
      <td>用于用户发起退款</td>
   </tr>
   <tr>
      <td style="text-align:center;">支付设置</td>
      <td></td>
      <td>用户可自主排序支付顺序、支付方式</td>
   </tr>
   <tr>
      <td style="text-align:center;">会员服务</td>
      <td></td>
      <td>帮助用户在特定时间预定场地、支付时优惠力度更大等</td>
   </tr>
   <tr>
      <td style="text-align:center;">意见反馈</td>
      <td></td>
      <td>收集用户使用APP的反馈</td>
   </tr>
   <tr>
      <td style="text-align:center;">在线客服</td>
      <td></td>
      <td>用户可点击联系在线客服</td>
   </tr>
   <tr>
      <td rowspan="4" style="text-align:center;">场馆详细页</td>
      <td style="text-align:center;">收藏</td>
      <td></td>
      <td>用户可收藏当前运动场馆</td>
   </tr>
   <tr>
      <td style="text-align:center;">文字展示</td>
      <td></td>
      <td>用简短的文字多方面介绍场馆</td>
   </tr>
   <tr>
      <td style="text-align:center;">图片展示</td>
      <td></td>
      <td>用清晰的图片对场馆、所能预约的场地进行展示</td>
   </tr>
   <tr>
      <td style="text-align:center;">预定选择</td>
      <td></td>
      <td>用户点击后进入预约界面</td>
   </tr>
   <tr>
      <td rowspan="4" style="text-align:center;">预定界面</td>
      <td style="text-align:center;">选择时间</td>
      <td></td>
      <td>用户可选择想要预约的时间</td>
   </tr>
   <tr>
      <td style="text-align:center;">选择场地</td>
      <td></td>
      <td>用户可选择当前场馆所能预约的场地</td>
   </tr>
   <tr>
      <td style="text-align:center;">预定信息</td>
      <td></td>
      <td>用户需完善预定时间、人数、联系方式等信息</td>
   </tr>
   <tr>
      <td style="text-align:center;">支付</td>
      <td></td>
      <td>用户在完善预定信息后支付订单</td>
   </tr>
   <tr>
      <td rowspan="5" style="text-align:center;">注册页</td>
      <td style="text-align:center;">手机验证码登陆</td>
      <td></td>
      <td>用户可直接通过手机验证码注册、登陆</td>
   </tr>
   <tr>
      <td rowspan="3" style="text-align:center;">其他账号登陆</td>
      <td style="text-align:center;">QQ</td>
      <td>用户可通过QQ账号一键登录</td>
   </tr>
   <tr>
      <td style="text-align:center;">微信</td>
      <td>用户可通过微信账号一键登录</td>
   </tr>
   <tr>
      <td style="text-align:center;">Apple</td>
      <td>用户可通过Apple账号一键登录</td>
   </tr>
   <tr>
      <td style="text-align:center;">用户协议</td>
      <td></td>
      <td>用户使用APP前需了解并同意《用户协议》《用户隐私协议》</td>
   </tr>
</table>

#### 2、原型界面
#### 3、原型页面的流程图
### （三）API调用
#### 1、运动场馆地址
#### 2、智能推荐
#### 3、人脸识别
部分场馆可人脸识别入馆。

1、API使用/编程功能的基本描述
（200-250字 写给没有上过课的人，介绍此项目的具体实践思路、方法，可能需要的学习成本（时间成本大概要多久。）
（最好融合两种知识领域，计算思维/编程思维和设计思维及相关专业可能会用到的需求
2、云端项目部署的基本描述？
用云开发进行部署，提供开发部署的所有数据集合，绘制不同数据集合并介绍结构图，作简要的页面功能介绍，精简介绍云端功能和部署心得。（脑图）


## 三、学习/实践心得总结及感谢
### （一）实践心得
项目初期，我结合运动爱好，并通过对价值主张设计相关知识的深度学习，对产品做了详细的需求分析以及设计方案。

随后，在价值主张画布的基础上，我通过界面设计、功能设计、选择合适的API，努力实现价值主张和客户工作、痛点和收益契合的第一阶段——书面上问题-方案契合。

我在实践的过程中不断进步，同时也了解到我所拥有的知识仅是皮毛，仍要进一步学习。
### （二）感谢
能够完成本项目，我十分感谢许智超老师以及强大的互联网资源，以及感谢《价值主张设计：如何构建商业模式最重要的环节》这本书和它的独家资源。

移动互联网开发课程能够帮助我们学习移动互联网产品的开发，通过完成这一个项目的开发，我了解到要开发一个产品的准备工作是十分复杂的。学无止境，我们应该主动学习更多相关知识，并学会更熟练地运用他们。

参考链接：
