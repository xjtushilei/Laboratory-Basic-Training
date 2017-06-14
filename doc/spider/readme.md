#　Spider


了解最基本的爬虫

1. 下载html （http协议）
2. 解析 （css，xpath，正则表达式）
3. 存储 （txt，mysql，MongoDB）

# Jsoup

一个集下载和解析为一体的jar包。

资料：http://www.open-open.com/jsoup/

其中重要的是 使用选择器语法来查找元素 ：http://www.open-open.com/jsoup/selector-syntax.htm

**演示**：如何使用谷歌浏览器进行选择元素

# 框架

## 1.WebMagic

官方中文文档：http://webmagic.io/docs/zh/

按照文档流程走下来，很舒服的。

## 2.ScriptSpider

https://github.com/xjtushilei/ScriptSpider

自己挖的一个坑。大的bug没有，需要完善很多。主要是当时分布式的不多，才下的手，后来太忙没有继续下去。结合spring-boot的思想，简洁就是好。

## Python

java爬虫方面不是很友好，最大的就是java不是脚本语言，不方便，不支持类型推断等等。java在行的主要是web领域。介绍一些python的爬虫。

### 1.beautifulsoup

和jsoup一模一样。

### 2.scrapy

爬虫的最高境界。主要是社区比较好，发展的很好，你能想到的功能都有。由此可见，社区很重要，不管你的产品有多好，没有被推广起来也不行。

# 要求

- 爬取交大新闻网的新闻100条，存到txt。（推荐使用 Apache 的 commons-io.jar 包）
- 爬取百度百科这[100个人](names.txt)的信息。把一些通用的信息（性别，年龄之类的）抽取出来，存到mysql中。