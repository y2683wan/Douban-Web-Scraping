# **豆瓣爬虫**
## 使用的库/框架 Library/Frameowrk Used
* os 
* time 
* pandas       
* selenium   
* requests   
* BeautifulSoup     
                                                                                                                                    
## **1. DoubanGroupMemberSpider.ipynb**
根据豆瓣小组ID爬取所有该豆瓣小组所有成员的信息 
* 用户ID
* 用户名
* 用户主页URL
* 地点(optional))


## **2. DoubanPostCollector.ipynb**
根据豆瓣小组ID爬去取所有该豆瓣小组的所有精华帖数据 （reuqest)
* 精华帖的正文文字信息 txt
* 精华帖的正文链接 csv txt
* 精华帖中的图片/动图 按照出现顺序标号命名
* 精华帖的评论信息 (评论ID， 评论内容) csv txt
* 精华帖的pdf

数据量大的时候，使用request会触发豆瓣的反爬机制


## **3. DoubanSpider-selenium.ipynb**
根据豆瓣小组ID爬去取所有该豆瓣小组的所有精华帖数据 (selenium)
* 精华帖的正文文字信息 txt
* 精华帖的正文链接 csv txt
* 精华帖中的图片/动图 按照出现顺序标号命名
* 精华帖的全部信息截图

通过selenium解决反爬的问题
login可通过手动扫描二维码或者find_element_by_class_name().click来解决
一旦登录不会出现反爬的问题


## **4. Group712168 Folder**
爬取小组结果demo
根据帖子的标题创建路径，整理爬取的数据信息

## **5. Copyright**
DoubanPostCollector.ipynb 中使用的代理来自快代理
> https://www.kuaidaili.com/free/
