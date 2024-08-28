# qidian_analysis

@author: <a src="https://github.com/yizhishiliu">shiliu</a>

### 目的

本次的数据分析项目实现了数据爬取、解析、储存、分析和可视化等需求。本项目整体使用了Python语言，爬取的目标是起点中文网，目的是获得其畅销榜单的100部小说的相关信息（排行，书名，作者，书籍类型，简介，最新章节，最近更新时间和书籍链接），并在网页上进行相应的分析和可视化展示。

### 介绍

- spider_qidian：将目标网站的数据进行爬取、清洗，然后保存在excel和数据库中


- flask_qidian：web可视化展示


- 本次项目实现的大致功能：

    1. 网页爬取：采用Python中的urlib库连接并且爬取了起点中文网畅销榜单，获得了需要的内容。
    
    2. 数据解析：利用了BeautifulSoup和正则式对获取的网页内容进行了解析，拿到我们需要的信息（排行，书名，作者，书籍类型，简介，最新章节，最近更新时间和书籍链接）。
       
    3. 数据存储：将拿到的数据保存在了Excel文件中同时也利用sqlite3库将相关的数据保存在了数据库中，以便于之后数据的利用。
       
    4. 数据分析：利用flask框架构造了一个本地的网站，再次利用sqlite3操作数据库进行数据分析并且在网页上进行了展示。
    
    5. 数据可视化：通过echarts对书籍类型分布情况绘制了柱状图，然后又用wordcloud完成了对书籍简介词频分析和图像的制作，同时进行了展示。
    
### 环境

python3.9 + BeautifulSoup4 +flask + 各种库

### 搭建/运行

1. 数据爬取(指定起止页1~20)

![image](https://github.com/user-attachments/assets/a122350f-297d-415f-a399-d609a6bc4a69)


2. 可视化展示(运行app.py后访问终端显示的链接)

![image](https://github.com/user-attachments/assets/ba12741b-b4e3-4064-b3d0-429476f1083b)


### 效果图

1. 首页(轮播图)

![image](https://github.com/user-attachments/assets/8fc0e681-cbe7-4c94-a6a4-6b61ed9113c5)


2. 书籍(畅销榜)

![image](https://github.com/user-attachments/assets/2ca976d1-cfde-49c3-b033-cfc818de6016)



3. 柱状图(类型分布)

因为后面测试清空了，后面随便爬取了几页作为演示参考，数据较少

![](https://github.com/Mingdaj/qidian-analysis/assets/130920375/e1a6a546-7d2d-4a6e-8a02-d8f6dcab992e)

4. 词云

![image](https://github.com/user-attachments/assets/4dbdc87f-504c-4819-9e7e-f9f65851e024)


5. 图书类型再分类分析

![image](https://github.com/user-attachments/assets/7027d3c9-1f45-4a27-94b4-8ec336529e95)


6. 可视化大屏

时间比较紧这里就随便做成了静态的，替换数据即可。如果需要动态大屏，请访问这个仓库：[https://github.com/yizhishiliu/qidian-visual](https://github.com/yizhishiliu/qidian-visual)

![](https://github.com/Mingdaj/qidian-analysis/assets/130920375/5c9116e8-8d77-49d3-b895-0b925c47d640)


天下没有免费的午餐，前后端代码+部署调试搞活动，详情加V咨询。前10名购买半价，另外有一些学习问题也可以一起交流，买到就是赚到！

点我+V](https://github.com/yizhishiliu/yizhishiliu/blob/main/images/wechat.jpg)
