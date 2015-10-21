# Python 培训计划
### 在线教程
* 廖雪峰: http://www.liaoxuefeng.com/wiki/0014316089557264a6b348958f449949df42a6d3a2e542c000
* 慕课网 Python入门：http://www.imooc.com/learn/177
* 慕课网 Python进阶：http://www.imooc.com/learn/317
* Runoob：http://www.runoob.com/python/python-tutorial.html

### 阶段
分为`Python入门`，`Python进阶`和`Python实战`

#### Python入门
Python是什么语言，能做什么。  
Python的特点是什么（脚本、解释型语言；丰富的内置、第三方库；快速原型开发）  
基本语法，变量类型，特殊运算符，特殊语句（如pass）  
集合类型（list、tuple、dict、set），函数定义

#### Python进阶
切片，迭代器，列表生成式  
面向对象，模块，正则，多线程，多进程  
函数式编程（map/reduce；filter；sorted），装饰器

#### Python实战
安装、使用第三方库  
爬虫，多线程(进程)数据处理  
SQL，Celery，Flask，Requests，BeautifulSoup等库

### 作业
#### 1. 计算+，-，*，/，()和0到9数字组成的算术表达式
**要求：**  
命令行输入输出  
输入表达式字符串，如：`1*2+(3-6/3)*4`  
输出有两行，第一行为逆波兰式字符串：`12*363/-4*+`，第二行为表达式结果：`6`  
**提示：**  
用`调度场算法`算法将输入的中缀表达式转换成逆波兰式；用list模拟栈数据结构。  

#### 2. 统计文章词频
从 [http://pan.baidu.com/s/1bnr072f](http://pan.baidu.com/s/1bnr072f) 下载小说集合，提取密码：2yea  
对小说集合中的所有文章做分词，统计词频。  
用结巴分词库做分词：[https://github.com/fxsjy/jieba](https://github.com/fxsjy/jieba)   
结果保存在sqlite数据库里面。  
至少保存词和词频  
**思考**：考虑如何用多线程、多进程加快速度；思考如何运用MapReduce思想解决这个问题。

#### 3. 网页内容爬取
爬取 [唐巧的技术博客: http://blog.devtang.com/blog/archives/](http://blog.devtang.com/blog/archives/) 所有文章  
用多线程爬取。  
将爬取内容保存在sqlite数据库里，要保存文章的标题、时间和正文。  
Http请求库：[Requests: http://docs.python-requests.org/en/latest/](http://docs.python-requests.org/en/latest/)  
解析Html的库：[Beautiful Soup: http://www.crummy.com/software/BeautifulSoup/](http://www.crummy.com/software/BeautifulSoup/)  
**注意**：多线程下sqlite的读写问题。  
