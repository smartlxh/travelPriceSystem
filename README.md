#travelPriceSystem
#author:smartlxh
   整个系统总体分为三个模块，分别是爬虫模块，数据库模块和web模块。实现分布式爬虫同时爬取指定的在线旅游网站，然后能够将爬到的数据进行预处理，然后将处理过的结构化数据存到数据库系统里。同时爬虫的爬取频率和时间是可以设置的。采用Mongodb数据库集群，能够将爬虫获得的数据路由到合适的服务器上，实现负载均衡。当用户在网站上查询时，web服务器向数据库请求数据，然后将获得的数据通过一系列的比价决策最终将结果返回给用户一个推荐列表。如果用户选择了任意一个方案，web系统会收集这个用户的选择信息，然后用来对比价决策训练数据，从而优化比价决策，作出更准确的推荐。
