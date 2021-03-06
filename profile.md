# 简历


## 基本信息

* 姓名：曹志攀
* 性别：男
* 出生日期：1991-01-11
* 手机：13120358448
* 邮箱：13120358448@163.com
* 大学：北京联合大学
* 毕业时间：2014-07

## 工作经历

* 百度游戏(2014-07~2015-04)
* 一亩田(2015-04~now)

## 项目经历

* 微信公众号

  ```shell
  # 开发语言：php
  # 优点：微信公众账号高度封装，分分钟响应日常运营活动
  # 缺点：框架设计有点随意，另外微信公众号当时接口变动频繁不能及时响应，监控不足，没有配置后台
  ```

  ​

* push

  ```shell
  # 开发语言：golang
  # 涉及模块: mq_server, dispacher, ob, channel_server
  # 主要负责ob和channel_server的开发
  # 存储：redis
  # 优点：健壮，扩展性极强，push机制和notify机制结合，很好的平和了消息到达率和即使度，很容易对接新的推送渠道
  # 缺点：监控不完善，apns推送缓慢
  ```

  ![基础架构](http://thumbnail0.baidupcs.com/thumbnail/4a8e7cf64bc46012c5af709d8c07bf10?fid=1327980910-250528-898047007383025&time=1466521200&rt=sh&sign=FDTAER-DCb740ccc5511e5e8fedcff06b081203-ChJbnqkXCWmadDEk22csgubv%2FLI%3D&expires=8h&chkv=0&chkbd=0&chkpc=&dp-logid=4011828411118754103&dp-callid=0&size=c710_u400&quality=100)

  ​

* im

  ```shell
  # 开发语言：golang,php
  # 涉及模块: chart, msg, proxy
  # 主要负责 chart, msg模块 及部分proxy接口开发
  #存储：redis, mysql, mongodb
  # 优点：只做消息存取，扩展性强，结合push系统能使消息尽快到达用户
  # 缺点：过于依赖redis，存储分散，迁移数据麻烦
  ```

  ![基础架构](http://thumbnail0.baidupcs.com/thumbnail/a3ba2ee61d41ae6226156cdf0f9b80cc?fid=1327980910-250528-1070667201037587&time=1466521200&rt=sh&sign=FDTAER-DCb740ccc5511e5e8fedcff06b081203-UlU2Fpfx6vKOwBTVKIh0pzxIzdA%3D&expires=8h&chkv=0&chkbd=0&chkpc=&dp-logid=4012011186754550537&dp-callid=0&size=c710_u400&quality=100)

* call

  ```shell
  # 开发语言: php
  # 对接服务：云通讯，有信，吉亚通讯
  # 主要模块：用户拨打记录接口，渠道回调接口，通话记录及录音下载, 监控
  # 优点：有效避免用户手机号泄露，通话记录有据可查以防交易纠纷，方便接入新的电话渠道
  # 缺点：由于第三方服务的问题，通话质量一直饱受诟病
  ```

  * 用户画像

  ```shell
  # 开发语言：php, python, shell
  # 开源工具: hadoop(streaming), sensors(其实不适合做数据仓库)
  # 模块：collection(收集数据), deal(预处理), tag(计算标签), out(输出数据－》 mysql, redis, crm ....) ,api
  # 主要负责：ALL
  # 标签分类：静态标签(用户基本信息), 常在位置，常用供应位置，关心品类，用户角色(买家卖家), 主营品类，买家等级(需要继续挖掘), 活跃度，熟练度，服务质量。。。。
  # 优点：架构简单，模块间耦合性低，筛选方便，能够快速响应各种需求
  # 缺点: 开发过程中优点随意，虽然该架构能够兼容各种开发语言，但给别人维护的时候可能会有坑
  ```

  ![基础架构](http://thumbnail0.baidupcs.com/thumbnail/7d9d1ff81f37ef048078be13ed2b3b5e?fid=1327980910-250528-1084118321205671&time=1466524800&rt=sh&sign=FDTAER-DCb740ccc5511e5e8fedcff06b081203-WGeUsCB2QgLunCpkXCNzPJdBZ%2Fw%3D&expires=8h&chkv=0&chkbd=0&chkpc=&dp-logid=4012507651895683709&dp-callid=0&size=c710_u400&quality=100)


* 短文本分类探索

  ```shell
  # 懵懂阶段：使用一批买家聊天记录作为样本，使用svm算法训练之，3个小时之后测试准确率发现只有7%
  # 懵逼阶段：随机取出10000条聊天记录 使用k-means算法聚类，破机器上跑不动，然后取5000条记录，发现50个簇时向量距离为2400...
  # 憧憬阶段：发现随机1000条聊天记录和5000条记录（去掉数字）切词后次数都为5700左右，所以可以先对这5700个词手动分类（位置，货品，联系，人名，价格，问候。。。）得到一个初始语料库，然后基于词频对每一条聊天记录向量化，然后使用k-means聚类得到初始样本，再使用svm对聊天记录预测分类
  ```

  ​

## 语言

* php（就是简单, 比较适合快速搭建中间层接口及web应用）
* golang（设计思想很nb 天生协程，错误处理机制, reflect，跨平台免编译，自带doc机制。。。但是有很多吐槽点如开源包管理，代码怎么看都不够优美 ）
* python （神器，最近才接触，代码优雅，使用简单，文档齐全，社区活跃，溢于言表）
* html 
* javascript
* shell(搭配python效果更佳)



### 简历链接:https://github.com/caozhipan/myDoc/blob/master/%E7%AE%80%E5%8E%86.md](https://github.com/caozhipan/myDoc/blob/master/%E7%AE%80%E5%8E%86.md)



