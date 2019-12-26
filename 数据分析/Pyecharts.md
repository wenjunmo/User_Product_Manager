<div align = "center">
<h1>:whale2: 交互式数据可视化 :whale2:</h1>
<p>[pyechart 官方文档](https://pyecharts.org/#/)</p>
<p>[plot.ly 官方文档](https://plot.ly/python/getting-started/#initialization-for-online-plotting)</p>
</div>

### week01 

预热:
- [https://rawgraphs.io/](https://rawgraphs.io/) ==> Start [https://app.rawgraphs.io/](https://app.rawgraphs.io/) ==> try your samples - - example: 电影数据 - 冲积图 - X轴流派和电影 + y轴生产预算（百万）

安装 Pyecharts 踩到的坑
1. [pip install pyecharts-少 future 包- Read Time out-缺少 pillow 包，安装好后使用 IDLE 导入 Pyecharts 包或者直接在 python 安装目录下的 Lib\site-packages 文件夹里面查看是否存在 pyecharts 文件夹，这个应该是v0.5的版本，现在已更新到v1.0版本，两者是互不兼容需要查看官方文档来进行安装](https://zhuanlan.zhihu.com/p/28329657)
2. [import pyecharts 导入报错问题](https://www.codeleading.com/article/67112288373/)
3. [from example.commons import Faker 报错 issue 有讲是版本前后更新的问题，但是不够具体必须去查官方文档](https://github.com/pyecharts/pyecharts/issues/1393)
4. [pyechart GitHub README.md 写到 v0.5.x 和 V1 间不兼容,新版本系列将从 v1.0.0 开始，仅支持py3.6，文档位于 pyecharts.org，pip 安装命令如下:安装 v1 以上版本 $ pip install pyecharts -U ， -U 是和没有-U区别开来，也就是0.5与1.0版本的区别](https://github.com/pyecharts/pyecharts)
5. [pyechart 与jupyter 交互式，图表显示空白的解决方案](https://blog.csdn.net/zqs305082800/article/details/84581299)
6. [Anaconda找包，安装包时，遇到PackageNotFoundError： ''Package missing in current channels"](https://blog.csdn.net/ksws0292756/article/details/79192268)
7. [ImportError: No module named 'pyecharts' 使用pypi包链接路径安装](https://blog.csdn.net/skj1995/article/details/81187954)
8. [python -m pip install --upgrade pip 升级后再来pypi进行安装]-Segmentfault](https://segmentfault.com/a/1190000018129346)
9. [官网pyecharts 0.1.9.4 pip install pyecharts==0.1.9.4Copy PIP instructions](https://pypi.org/project/pyecharts/0.1.9.4/#files)
10. [pip install pyecharts-0.1.9.4-py2.py3-none-any.whl](https://blog.csdn.net/f823154/article/details/80671072)

总结：
1. 出现这么多问题两种解决办法：一是看官方文档来对pyecharts的官方文档进行下载版本修改，而是在pypi网站上直接下载包到本地再解压或者直接cmd解压包所在的网址
2. 关于 anoconda jupyternotebook 生成的 Html 文件图片全部丢失原因是在默认生成的Html文件是储存在C盘的下载里面，下载好后必须要将文件移动出去，否则会一直重复下载相同文件没有办法来显示图片，导致只有代码没有生成图的奇怪现象
3. pyecharts在jupyter上无法使用，jupyter notebook总是显示没有模型pyecharts，问题是已经安装了包，而且在pycharm里可以运行，应该是版本问题使用的pip命令下载包并没有 -U 来下载最新的 v1.0

>工厂函数：class类，type类，两个不一样，召唤魔法，掌握程度不一样，web app 对象，对象值的差别，同样一类东西召唤出来就是不一样的。import pandas 召唤数据库里面最常用的数据对象就是pd.DataFrame，常用方式就是df=，每一次召唤一个数据框的对象做一个副本来做一个数据框，pd.DataFrame 后面产生一个数据框和索引，单位index

csv档放在目录下面就是来进行
read.table/csv
看不到数据框就是
列表字典或者字典列表生成一个数据框

面向对象

MVC框架https://baike.baidu.com/item/MVC%E6%A1%86%E6%9E%B6/9241230?fromtitle=mvc&fromid=85990
数据视图
带来python课本来复习mvc和类别概念，把df再来清楚，召唤数据的源头 

flask模块

类-召唤能力，生儿子
叫出来的数据框是不一样的

pychart
召唤chart对象，与已有东西有发生什么东西
对应的是barcharts
列表的数据
用pandas模块召唤出数据框欧盟28国和碳排放，跳出数据丢到pychart的交互可视化
召唤的是条形图，数据在里面

类型图里面，累加性
flask pandas pycharts 

魔法就是咒语，都是工厂，看pycharm
实例：实在的例子

给出数据给出函数就是可以召唤出魔法，背下来这张图最基本的编程能力
面向对象

工厂力就是把类型数出来

强烈的图形印象
实例时工厂预先设定好的数据集和方法，可以抽数据
数据框抽出来喂给它做

工厂在中间那一页

生成的工厂函数
faker假的 产生随机数据
pychart里面有一些选先

怎么召唤出来

[柱状图](https://pyecharts.org/#/zh-cn/rectangular_charts?id=bar%ef%bc%9a%e6%9f%b1%e7%8a%b6%e5%9b%be%e6%9d%a1%e5%bd%a2%e5%9b%be)

每次召唤就是
实例召唤
人生不要太混，太混就没有了





pd不行是因为你没有把文件放在初始目录下面，所以就是不行启动


后面是这样子解决的
就是你的正在编辑的ipynb文件一定要和想要读取的csv文件在同一文件夹里面，或者找到之前的代码来进行复习
接着就是可以在同一目录下面来打开代码了
其实就是一个需要
找到上学期学习的pandas来进行学习

[Jupyter notebook如何打开数据集](https://blog.csdn.net/wangdan113269/article/details/79609248)
[ipython notebook 如何修改一开始打开的文件夹路径？](ipython notebook 如何修改一开始打开的文件夹路径？)
[如何用Jupyter notebook打开本地数据集](https://www.cnblogs.com/annage/p/9430394.html)
[python读取CSV文件时的路径](https://blog.csdn.net/u010084228/article/details/78110145)
[读写文本数据](https://datartisan.gitbooks.io/begining-text-mining-with-python/%E7%AC%AC3%E7%AB%A0%20%E6%96%87%E6%9C%AC%E6%95%B0%E6%8D%AE%E6%9D%A5%E6%BA%90/3.4%20%E8%AF%BB%E5%86%99%E6%96%87%E6%9C%AC%E6%95%B0%E6%8D%AE.html)
[处理CSV文件和JSON数据](https://www.osgeo.cn/python-tutorial/textfile-CsvModule.html)
[“ CSV文件不存在”-Pandas Dataframe](https://stackoverflow.com/questions/39267614/csv-file-does-not-exist-pandas-dataframe)


[pandas中关于set_index和reset_index的用法](https://blog.csdn.net/jingyi130705008/article/details/78162758)
DataFrame可以通过set_index方法，可以设置单索引和复合索引。 
DataFrame.set_index(keys, drop=True, append=False, inplace=False, verify_integrity=False) 
append添加新索引，drop为False，inplace为True时，索引将会还原为列

reset_index可以还原索引，重新变为默认的整型索引 
DataFrame.reset_index(level=None, drop=False, inplace=False, col_level=0, col_fill=”) 
level控制了具体要还原的那个等级的索引 
drop为False则索引列会被还原为普通列，否则会丢失

[Python 基本操作- 数据选取loc、iloc、ix函数](https://www.jianshu.com/p/1115699e0674)



[国家统计局](http://www.stats.gov.cn/)
[pandas 基本操作记录](https://www.jianshu.com/p/d80e0e690f3d)

在国家统计局里面找到csv利用pandas打开来看数据，
[https://pyecharts.org/#/zh-cn/assets_host](https://pyecharts.org/#/zh-cn/assets_host)
资源引用


faker

[用python3读csv文件，出现UnicodeDecodeError: 'utf-8' codec can't decode byte 0xd0 in position 0: invalid con](https://blog.csdn.net/moledyzhang/article/details/78978312)

[pandas读取csv处理时报错：ParserError: Error tokenizing data. C error: Expected 1 fields in line 29, saw 2](https://blog.csdn.net/yj928674542/article/details/75634197)

tableau的图标
散点图基本发问：x轴y轴两个变量的相关性，不是每个相关性都是很明显的
gdp和摊牌的，越来越好
趋势线，相当碳排gdp会排放更好
广州
经济学：经济和生态的脱钩，经济发达不需要碳排，网页制作两三章图来进行页面交互，把3门课以上做有意义有帮助有整合激素hi可以做了：py，大数据，tableau 多做和思考和论点需要两三个论点，来自于拿一些不同的数据和图标可以说出一套数据
散点图：
直线折线和地图
程序库pradesk

基本阅读文档和基本的处理能力
前端代码不会写就是可以用现成的模块化工具，产品经理加数据分析师，做出来的图可以给前端来优化，整合能力给自己标准高一下，就是核心人员

作业：分省年度数据，地区代码，tableau也有数据
分省年度数据把他地图可视乎啊讲出相应的数据

11号交
12月设计，额外教学画出来，全世界个国家的碳排，折线图和柱状图，特殊展示图片列入


作业参考文档

[DataFrame.loc](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.loc.html)
[pandas 基本操作记录](https://www.jianshu.com/p/d80e0e690f3d)
[Pandas DataFrame 的基本操作之重新索引](https://blog.csdn.net/baishengxu/article/details/81349451)
[pandas重新生成索引](https://blog.csdn.net/tongjinrui/article/details/80619838)
[https://pyecharts.org/#/zh-cn/rectangular_charts](https://pyecharts.org/#/zh-cn/rectangular_charts)


出现错误的解决办法：
[pandas.DataFrame.set_index](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.set_index.html)
[pandas读取csv处理时报错：ParserError: Error tokenizing data. C error: Expected 1 fields in line 29, saw 2](https://blog.csdn.net/yj928674542/article/details/75634197)
[python中报错：SyntaxError: invalid character in identifier](https://blog.csdn.net/wushaowu2014/article/details/78305232)
[pandas 基本操作记录](https://www.jianshu.com/p/d80e0e690f3d)
[python错误之SyntaxError: invalid syntax](https://blog.csdn.net/zcf1784266476/article/details/71335939)
[Python中pandas dataframe删除一行或一列：drop函数](https://blog.csdn.net/songyunli1111/article/details/79306639)
[pandas删除（drop）方法](https://blog.csdn.net/sinat_32547403/article/details/73822660)
[python pandas读文件(不把第一行作列属性)也就是header属性](https://blog.csdn.net/SZU_Hadooper/article/details/78913644)
[暂时还找不到'DataFrame' object has no attribute 'conlumns']()


#### #第9周-使用世界银行提供的数据来进行世界地图可视化操作#

[世界银行数据库](https://data.worldbank.org.cn/)
[使用说明文档](https://data.worldbank.org.cn/about/get-started)

[老师案例](https://population.un.org/wpp/Download/SpecialAggregates/EconomicTrading/)

1.要求：在世界银行提供的数据库下载数据后进行清洗再导入 Pycharts
2.我选择了


先来安装第一步：
    
    pip install faker

发现了版本不对就来安装

    python -m pip install --upgrade pip

但是还是被显示了这些东西

    WARNING: You are using pip version 19.2.3, however version 19.3.1 is available.
    You should consider upgrading via the 'python -m pip install --upgrade pip' command.

您正在使用pip版本19.2.3，但是版本19.3.1可用。
您应该考虑通过“ python -m pip install --upgrade pip”命令进行升级。

    pip list
有pyecharts                          1.5.1

在conda里面更新

    conda install mingw libpython



识字率，青年总体（占 15-24 岁人口的百分比）https://data.worldbank.org.cn/indicator/SE.ADT.1524.LT.ZS
老年抚养比（占工作年龄人口的百分比）https://data.worldbank.org.cn/indicator/SP.POP.DPND.OL


必须是要使用英文的资料才是可以的不然没有办法来及逆行文件图形的展示九就是没有数据就是比较玛法

Literacy rate, youth total (% of people ages 15-24)https://data.worldbank.org/indicator/SE.ADT.1524.LT.ZS
这就是·英文的下载csv的链接


so 又要过来清洗数据

找到了一个宝藏

这个真的是一个宝库来的

[公共数据库介绍~联合国数据库UNDATA](https://blog.csdn.net/loveyy1010/article/details/72954949)

[http://data.un.org/](http://data.un.org/)
[dataset查找-un](http://data.un.org/Explorer.aspx)





[识字率](https://www.un.org/chinese/millenniumgoals/unsystem/indicator8.htm)



不像找了就直接写吧


 怎么使用GitHubdestop 与gitee使用

新建一个仓库，接着来克隆到本地端，接着将保存好的jupyternote文件变成了html文件下载后就是将名字改成了index.html文件就是来放在本地段克隆好的文件里面，接着就是来进行push提交后，就是来进行gitee的git page 生成一个网页就是看到了我们的juputernote的内容就是完全变成了可以再网页上面显示的一样了



https://data.worldbank.org.cn/indicator
这个是比的链接和指标

[企业信息披露程度指数（0 = 较少披露，10 = 较多披露）](https://data.worldbank.org.cn/indicator/IC.BUS.DISC.XQ)

这个是我抓取的数据

[python – 将Pandas DataFrame转换为字典](https://codeday.me/bug/20180414/152036.html)

这个是实验过程用到的数据

不知道为什么我的ipynb导出为html后就是显示不了图片生成的图就是非常奇怪
中午又要来进行检查


[数据可视化（三）- Seaborn简易入门](https://www.cnblogs.com/kylinlin/p/5236601.html)

[Seaborn教程](https://blog.csdn.net/leo00000001/article/details/70226600)




[30分钟学会pyecharts数据可视化](https://zhuanlan.zhihu.com/p/63236019)

按照这篇来进行

Python与算法之美公众号后台回复关键字：源码。获取本文全部代码。、
1，柱形图






[Python怎样简单画折线图饼图柱状图？](https://www.bilibili.com/video/av66336238?from=search&seid=4213445260121928891)
[【 数据可视化 】如何做数据可视化？（中文）](https://www.bilibili.com/video/av14732029/?spm_id_from=333.788.videocard.1)
[【 数据科学：使用plotly进行数据可视化 】Data visualization with plotly |](https://www.bilibili.com/video/av46798646?from=search&seid=16088863287642101713)
[Python数据可视化 - Plotly教程](https://www.bilibili.com/video/av70964692?from=search&seid=15136466416390666254)
[Python爬取数据并进行可视化展示](https://www.bilibili.com/video/av20319191/?spm_id_from=333.788.videocard.1)


11.22


maji搜索引擎介绍


plotly
怎么excel打开csv文档-数据-自文本/csv
两种方式来打开csv文档
1.直接在excel2019-数据-自文本/CSV直接来打开让后就是加载转换-关闭并上载就是变成了数据已经编辑好的款款power query
2.直接在数据-获取数据-传统向导（在文件-选项-数据-显示旧数据导入向导（从文本（旧）））里面找到文本（旧）打开文本文件csv就是可以进入csv打开步骤，分隔符号utf-8-逗号-常规完成就好了

na那边是确信值，是不属于湾区的所以就是没有，是使用vlookup函数来进行的


安装好confline 和 flask

导入数据
怎么打开csv文件复习pandas
怎么打开app.py文件 cmd

把全部的hurun的文件目录记好，使用cmd进入有app.py的目录里面，用anocondaprompt来打开，pwd显示目录，cd进入包含的目录，使用python app.py就是跑一大串代码Running on http://127.0.0.1:8000/ (Press CTRL+C to quit)
就是

在jupyternote中怎么来打开app.py文件

render_template就是放htmlcssjs档
get就是获取信息
flask是基于jinja2来进行
POST用户上传和选择

需要改两个档


11.29


flask 告知服务意图：静态和动态
https的书籍复习
定义到什么样子的界限

数据的传输
互联网响应请求的方式

url 域名和通常协定http https
get
put 提交内容summit

hurun method 一遍是没有s，一遍是由s
两个对应

左边和右边拦起来，左边是flask 
render_template 就是把模板额数据结合在一起
render_template里面参数哪里不一样，路口和结果result=datastric

第一杠是路径和方法，

丢得出去就是可以丢到网网页里面，
加个safe不然得华页面希纳是就是html码

the_plot
the_res
jinja模板

the_select_religion是怎样子的
option 是下拉选单
列表，有几个就是option就是由几个

互动性选单数据驱动的方式

plot_all自负床
data_str字符长

第一个迭代就是空的

只有一个额东西不同
路由不一样

有时候是目录
post之后的路由会是在哪里
点击按钮是哪个来决定

http的模型就是requesrt response
右边前端触发要求，
右边驱动
左边选单regions_available

第二个迭代：
先不要看正解

df那一行用pandas模块read_csv方法csv档案编码utf-8分隔符\t	就是按tab键就是斜号t

第三个是先出表
基本数据照读

df.to_html() 是dataframe是数据框数据科学家的好方法
数据框取出一栏的值拆掉练习
table tr td

迭代4互动过滤只要看某一区的就是可以过滤
regional_reasonal 选取某一个湾区就是指错的变数回传到伺服器选取数据和过滤数据
df.query某个语法和语言从数据框抽取数据过滤出来就是，常用的填值得方式region=''
就是如何用query过滤数据，非常多，df过滤出来的表，跑出结果交互还是没有做好

迭代5交互图
fig iplot画图和后台有成果.html像字符长一样内嵌入网页里面就是比较清晰了
