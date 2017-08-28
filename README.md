#IngeniousSearch
IngeniousSearch搜索技术为客户搭建搜索系统提供技术支持和定制化服务，系统具有高性能、高质量、高扩展性的特点，核心架构和技术国内一流互联网公司具有的水平。

##系统架构
系统包括数据同步系统ETDL和搜索系统，系统中每一个功能模块都支持集群化部署。
###数据同步系统ETDL
####数据抽取（Extractor）
    将数据从数据源读出，支持的数据源包括数据库、文件、其他后台服务等等；支持多数据源数据的合并。
####数据转化（Transformer）
    根据需求对数据进行格式、解析、计算等处理；
####数据分发（Dispatcher）
    支持多层流式分发、数据分片等；
####数据加载（Loader）
    支持统一加载逻辑和并行化加载。
###搜索系统
####负载均衡模块（Nginx）
    支持域名解析、Nginx请求转发为基础的负载均衡；
####高级搜索模块（AS，advanced search）
    与QP、BS、DS进行交互，对搜索数据进行合并、打分、排序、组装处理。
####基础搜索模块（BS，basic search）
    索引建立、检索、排序等
####数据搜索模块（DS，data search）
    搜索数据在线存储和检索；
####搜索词分析模块（QP，query processor）
    分词、特征值计算等；
####搜索建议模块（SS，search suggestion）
    提供搜索提示
####推荐模块（RC，recommendation）
    根据历史点击记录、搜索记录、个人信息进行精准推荐。

##技术特点和优点：
###支持海量请求、大数据量
    系统中全部支持集群化部署、数据分片，可线性扩展。
###稳定性高
    与业内高层次互联网架构一致，已经过多年检验。
###实时数据秒级更新
###搜索响应快
   响应时间在百毫秒级。
###系统全部采用开源组件实现，支持对客户开放源码
###相比其他开源搜索系统(ElasticSearch等)，方便进行业务融合。
##Demo
   共收集专辑(电影,电视剧)50000+，明星30000+的影视数据，建立类似于爱奇艺、优酷的视频搜索服务。如下为demo截图

![image]("https://github.com/mountaintaitiger/ingenioussearch/blob/master/images/1.jpg)
![image]("https://github.com/mountaintaitiger/ingenioussearch/blob/master/images/2.jpg)
