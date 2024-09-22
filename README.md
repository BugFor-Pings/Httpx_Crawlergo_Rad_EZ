# Httpx_Crawlergo_Rad_EZ
Httpx过滤存活url，对存活的URL进行爬虫，两爬虫互相弥补，随后搭配EZ的主动扫描。

优化重写的联动脚本
将目标放入targets.txt中过后
直接python launcher.py即可

1.使用Httpx过滤去除502响应的目标后进行保存为：httpx.txt
2.然后使用Crawlergo和Rad对httpx过滤后的存活目标进行爬虫
3.配合EZ扫描器对目标进行扫描

优化后优点：
相比网上许多文章的直接使用爬虫+扫描好很多了
httpx过滤下来的都是存活能打开的目标域名
然后对这些域名进行爬虫+扫描，极大的减少了无用域名(502响应)的扫描
扫描完成结果会保存到out文件夹中，以年_月_日_时_分_秒命名来保存
文件名如：2024_09_22_06_42_12.html（妈妈再也不用担心分不清楚目标是多久扫描的了）


具体EZ配置教程可参考官方文档:https://docs.ezreal.cool/docs/config
