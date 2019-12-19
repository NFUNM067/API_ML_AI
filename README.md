发布日期    | 2019-12-1 
---------|------
史诗名称     | 人脸考勤小程序
文件现状     | 进行中 
文件主人     | 莫欣妹 
领头的设计师 | 莫欣妹 
领头的开发者 | 莫欣妹  
领头的测试者 | 莫欣妹  


## （一）加值宣言

大学上课考勤是必须的，平时上课考勤方式都是通过课代表一个一个名字念过，学生喊“到”的低效率考勤过程。然而，课代表念名字考勤期间还会出现念错名字、答了“到”课代表没有听到，同学代替别人答“到”（考勤作弊）等因为人工操作不当所带来的错误；其次，随着一个一个名字念过，浪费了课堂时间，影响了教学质量。但是随着人工智能的发展，针对大学生课堂考勤失误、考勤作弊、考勤效率低的痛点，现将采用高德API和百度人脸识别API针对用户痛点做出的产品进行加值和优化。主要：运用机器学习中人脸识别中的人脸对比和活体检测功能，通过识别图片中的目标用户是否为活体「真人」，比对识别图片中的目标用户与信息采集库中的目标用户图片中人脸的相似度，并返回相似度分值。辅助：还运用了百度地图API中的定位功能，对目标用户实现实时及精准的定位。


## （二）核心价值宣言（最小可行性产品）

着眼于用户的最基本需求，解决大学生课堂考勤失误、考勤作弊、考勤效率低的问题，给用户提供有针对性的人脸考勤的最基础服务，开发一个低成本，高效率，防作弊的智能考勤小程序。

## 用户痛点宣言

**背景：**

现在课堂考勤的必须的，但是平时考勤方式一般是人工考勤，人工考勤会经常会出现考勤失误、考勤作弊、考勤效率低的问题。所以，能够为课堂考勤提供有针对性的人脸考勤最基础服务，开发一个低成本，高效率，防作弊的智能考勤小程序，是为要进行课堂考勤的用户提供的好帮助。

**用户：**

大学生和老师

**目的：**

开发一个低成本，高效率，防作弊的智能考勤小程序

**用户痛点：**

- 场景一：课堂考勤时，课代表念错名字，导致某同学没有听清楚是自己名字；某同学答了“到”课代表没有听到，误记录了某同学旷课。
- 场景二：课堂考勤时，某同学帮助逃课的朋友答了“到”，课代表并不知道答“到”的不是逃课某同学本人，所以以为逃课某同学来上课了。（考勤作弊）
- 场景三：某专业课上进行课堂考勤，但是由于考勤人数多，用了15分钟考勤，导致老师课堂内容没有讲完，影响了教学质量。


## （三）AI概率性考量

- 百度人脸识别的人脸对比和活体检测技术，有三大保证：

1. 服务高效稳定：提供企业级稳定、精确的大流量服务，拥有较高可用性、弹性灵活的高并发承载，可靠性保障高达99.99%
2. 高精度识别：百度人脸识别技术国际领先，识别准确率超过99%，在多个国际公开竞赛排名第一
3. 响应速度快：人脸识别中的人脸比对和活体检测功能，支持百万级超大型人脸库，可实现毫秒级快速识别对比

- 所以，该产品利用了人脸识别中的人脸对比和活体检测通过现场获取用户人脸图片，进行人脸识别判断考勤结果。这两个功能技术不仅识别准确率较高，而且人脸识别速度以毫秒快速识别对比，2秒内完成人脸捕捉，普遍情况下都可以使用。该产品因环境因素或者拍照造成识别不准确的状况，概率较小为少数事件，对正面影响并不大。


## （四）需求列表

用户案列 | 对应标题 | 重要程度
----|------|----
某同学希望某节课上的考勤是可以快速完成，同时减少考勤错误的发生 | 人脸识别  | 重要
老师想要知道哪位学生考勤作弊了并逃课了 | 人脸识别  | 重要
老师想知道哪位同学考勤失败了 | 百度地图API  | 次重要 

**具体应用场景**

1. 上课时，老师要进行课堂考勤，老师觉得如果用一个一个名字念过，学生答“到”的方式考勤的话太浪费时间了。但是，老师发现最近有一个小程序可以帮助她高效率完成课堂考勤过程。于是叫同学拿出手机，打开人脸考勤小程序，让所有同学在人脸考勤小程序上通过人脸识别同时考勤，快速完成了课堂考勤。
2. 在上课的时候老师看到来上课的同学人数很少，进行了课堂考勤，然而课代表点完名后发现答“到”的人数比来上课的人数多了十几个。因为老师并不认识全部学生，所以并不知道哪位学生考勤作弊了。但是，老师发现最近有一个小程序可以帮助她很快找出考勤作弊的学生，于是叫学生打开人脸考勤小程序，快速完成了考勤，查看了考勤记录发现了考勤作弊的十几个学生是谁。


## （五）交互及界面设计

1. 登录/授权页面


![](https://github.com/NFUNM067/API_ML_AI/blob/master/login.png)

2. 刷脸考勤页面


![](https://github.com/NFUNM067/API_ML_AI/blob/master/face.png)

3. 考勤记录页面


![](https://github.com/NFUNM067/API_ML_AI/blob/master/records.png)

4. 我的页面


![](https://github.com/NFUNM067/API_ML_AI/blob/master/my.png)

## 信息设计 

信息设计：在PRD文件中是否有说明且原型是否有做到：信息设计的某个核心信息或设计使用了人工智能的加值

## 原型文档 

[原型文档下载区](https://github.com/NFUNM067/Product-document)

[原型文档交互展示](https://github.com/NFUNM067/Product-document)

## 口头操作说明

1. 该产品是个小程序，体量不会很大，不需要用户下载APP占用手机内存。
2. 该产品需求明确，需求针对的目标用户群体明确，是大学教师上课考勤学生防作弊小程序。
3. 该产品有核心功能和辅助功能，功能多样化。
4. 该产品解决了用户想要上课考勤节约时间并且防学生考勤作弊问题。

## 使用水平

## 使用比较分析

百度人脸识别技术，有三大保证：

1. 稳定性好提供24小时云端高稳定服务，宕机率低，故障恢复快，单图毫秒级响应，服务可用性高达99.95%
2. 准确度高：基于百度丰富的海量数据，利用深度学习技术及精准的算法迭代模型，不断提高准确性
3. 功能丰富：支持上千种物体识别及场景识别，并在持续增加中，让你更好的读懂世界。

所以，百度人脸识别提供6种在线/离线活体检测方案，支持图片质量校验、多帧图片识别，有效抵御照片、视频翻拍、3D模型等作弊行为。这利用高精度的人脸识别、对比能力，搭建考勤系统，提升考勤效率，提高防作弊能力

## 使用后风险报告

AI错误率：

目前人类对ImageNet图像的识别错误率大约在5%，微软的人工智能系统的错误率为4.94%，谷歌为4.8%。百度在2015年的时候已将这一错误率进一步降至4.58%，实现了质的飞跃。

错误现象处理办法：

1. 当人脸识别错误的话，可以手动输入不同处的关键词，帮助机器学习更正自己来给用户最正确的答案。
2. 当人脸识别失败的话，就用幽默的方式告诉用。第一次识别错误：‘因为近视无法识别清楚用户身份，请您在光亮充足的地方进行人脸识别’；第二次识别错误：‘因为学习不用功，忘记了这个东西的名称，可以发送反馈留言，后台客服妹妹将为您亲自解答。’

Update README.md

