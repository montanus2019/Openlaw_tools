# Openlaw Text-Analysis Tools
* 一个使用各类文本分析方法，来分析openlaw裁判文书的工具。
> https://github.com/IanHongruZhang/Openlaw_tools

* 由于开发者本人为一名数据新闻编辑，此工具是为制作数据新闻的稿件而制作。
详情请查阅澎湃新闻·美数课栏目的所有稿件，以及美数课栏目的网站。
> http://projects.thepaper.cn/thepaper-cases/839studio/?cat=4

* 可能曾经使用过该工具产生的稿件：
> 《为何有了“新解释”，纠错夫妻债务纠纷的历史遗案还那么难？》https://www.thepaper.cn/newsDetail_forward_3214161
> 《这是坑｜判决书中的微商骗局套路，微商可能比你更容易上当》https://www.thepaper.cn/newsDetail_forward_3139674
> 《图解｜中国式遗嘱：忌立遗嘱心态改观，遗嘱纠纷几时休》https://www.thepaper.cn/newsDetail_forward_2060254
> 《《巨额来电》套路深？图解462份判决书中的电信诈骗》https://www.thepaper.cn/newsDetail_forward_1902196

目前（2019-11-18）主要实现的功能有
* 筛去不符文本。
* 法条信息查找。
* 案件信息结构化重构。
* 使用正则表达式，对重要信息发掘并转换成html格式阅读。
* 词频分词。
* 自动摘要提取。（基于HanLp)
* 词语共现。（基于HanLp)
* 人名查找。（基于HanLp)
* 地名查找。（基于HanLp)
* LDA文书信息聚类
* Kmeans文书信息聚类
* Repeated-Bisection聚类（基于HanLp)

### 使用环境
* Anaconda 2019.10版本（至少是python3的发行版。）
* python3(所有ipynb文件在python3.7环境下写成。)
* 所需要的包都在requirements.txt里，若要单机使用：
> pip install -r requirements

### 使用方法
* 打开jupyter notebook，一路执行下去就好，会有交互的提示。

### 所要准备好的文件
* 从Openlaw（或者Openlaw API）中所下载下来的excel文件。
* 举例文件见于该repo中，如正当防卫、职业打假人等原表。

### 分文件解说
1.裁判文件API
* 此步借助openlaw API的平台来得到文书：http://develop.openlaw.cn/index.jsp
* 个人账号文书的每日上限是1000份文书，因此请控制下列代码运行时的条件。
* 获取文书的方法，也可以经由Openlaw的网站上按照条件下载，每个账号每天的限制为1000份。

2.

### 后续工作
* 做出web网页端的工具集成
