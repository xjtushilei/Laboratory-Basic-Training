# maven

这里是maven的学习以及了解！

在学习之前，建议您先学会简单的在您的项目中使用maven来管理包。

这开始之间，如果您听过这个小组分享[TeamShare-Maven.pdf](TeamShare-Maven.pdf),可以先回忆一下。




# 任务列表

请自行搜索相关技术，并完成下面的任务

### 1. maven 下载、安装、配置

Tips：
- 环境变量设置maven_home，而不要直接将bin目录丢进去系统path环境变量

### 2. maven 镜像


因国外的中央仓库下载太慢（1~20k/s），需要设置镜像(0.2~1.5M/s，视文件大小)。请自行寻找好用的国内镜像，在maven解压目录的config目录的settings.xml中配置。

Tips：
- 时刻（2017年5月2日）的阿里云镜像比较好用。

    ``` xml
    
    <mirror>  
            <id>nexus-aliyun</id>  
            <mirrorOf>*</mirrorOf>  
            <name>Nexusaliyun</name>  
            <url>http://maven.aliyun.com/nexus/content/groups/public</url>  
    </mirror> 
    
    ```

### 3. IDEA（ Coding 工具，或 eclipse ）的 maven 配置

Tips：
- 各个工具默认了一个config文件，所以需要这里修改，不然我们换镜像就没有意义了。
- 强烈推荐使用idea，需要license的请email到 xjtushilei@foxmail.com 



### 4. 搜索 `maven pom.xml` 学习想怪概念

大概浏览一遍就行，以后在实践中慢慢学习！

### 5. 使用 IDEA 创建第一个 maven 工程

创建过程中，学习pom.xml文件汇中 `artifactId` 、`groupId`等作用。

在dependencies依赖中增加 commons-io 和commons-lang包，推荐使用下面推荐的网站查询，并将依赖直接拷贝过来，并实际写一些这两包中他们的函数。

Tips：
- 第一次较慢，之后下载到本地的jar包就不会再次下载。
- maven 查询网站（推荐，更新稍有延时）：http://mvnrepository.com
- maven 官方查询（不推荐）：http://search.maven.org/
- 第一次请使用的packaging请选择：jar，之后如果有web工程需要再使用war


### 6. git to github

这一步，需要您先了解了git的基本使用。如果没有，maven 入门可以暂时停止了，请移步至其它。

在github创建一个工程项目！

利用idea的版本控制，将代码上传！

# 其他

## 系统学习资料

入门结束，如果有其他更加深刻的理解，可以参考：
- [易佰maven教程](http://www.yiibai.com/maven/)
- [史上最全pom详解](http://www.zuidaima.com/share/1781583829978112.htm)



