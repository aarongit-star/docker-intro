
# High level concept introduction

## 1. 老师介绍
- Yu Wang 老师--来自澳洲Atlassian公司
- Jira SRE manager
	主要工作确保 JIRA software 能够 24 X 7 正常运行

## 2. 几个部分  

第一部分：  巩固Devops的概念
   What (Devops 是什么)
   先 High level做个介绍

   WHY (为什么)
   举例：
	A business owner run a company , to run a website in cloud.   before  hire only one developer,  
after hire 10 developer  同时做网站的开发， 都同时做REALESE的时候，就会有CONFLICTS,如何更快更好的把FEATURE交付给客户。need more features and do the devlopment at the sime , conflicts might happen during release.

如果
火车理论：
	打比方每个火车就是同一个起点出发， DEVOPS 相当于一个 COORDINATOR，哪辆火车先出发，哪辆后出发 ， 
如果FEATURE的DELIVERY有BUG 可以让火车回到原点，让加速我们FEATURE的DELOPYMENT,  DEVOPS设计好铁轨，MONITOR好铁轨。如何加速FEATURE的流程，造铁轨

Devops解决的问题：如何加速FEATURE的DELO,如何让用户能够更快更好的最新DEV的FEATURE

！【DEVOPS CYCLE】()
这个循环中：
PLAN& CODE ----developer经常做的，DEVOPS需要了解知道，会做些CONFIGUREATION CHANGE 和开发
BUILD/RELEASE/DEPLOY/----主要DEVOPS engineer 做的 
OPERATE/TEST/MONITOR------SRE做的有些重合,test大家都会做一点
DEVOPS CYCLE 是一个CULTURE,  每天定时好几次部署， 自动化的流程做保障，需要系统的方案来做，帮助DEVLOPER做的东西交付给用户。

如何帮助公司提高效率，帮助DEV把产品更快更好的提交给用户


SRE的工作：产品交付给用户之后，用户会在软件上面访问测试等，会造成服务器的压力，来监控产品交付给用户后，他们运行的状态，来保证用户使用的工作正常。

SRE 的 工作 ：
小团队服务百万级用户使用云产品
服务器（电脑） ----它的CPU,DISK ,MEMORY是有物理极限的,不预测对方是如何使用， 很容易导致我们的系统崩溃

在以上这个循环中，需要掌握每个知识点。

展开细节：
Devops_Overview.drawio 流程图
 - 主要有3个DEV/STAGING/PRODUCTION
 - 其中 DEV/STAGING 主要做测试用的
 - 后面有MONITOR监控系统
 - CI/CD Pipeline
 - Devops的Practice 贯穿各个开发进程




第二部分： Docker

container 系统-----程序员只要专心写程序就好，不管底层的系统。更好的利用资源，轻量级。



What is Docker?
Why Docker?
	key words:  easily pack, ship, and run any application as a lightweight/isolated container which is easily distributable and can run virtually anywhere.
如图1：Docker 的使用会贯穿整个CI/CD的过程
	
![Alt text](images/cicdgitlab.png?raw=true)

--image repo 的作用 

举例：GOOGLE 数据中心， 一个REGION 几千上万的CONTAINER 如果有一个模板复制，就能方便部署时间更快，REQUEST 数量增多了， 可以很快增加CONTAINER的数量，部署之后MONITOR

KEY BENEFITS:
 *



第二部分内容：
## 4. Docker
### -4.1 Docker introduction
### -4.2 Docker handson -three major use cases
#### -Handson #1 ：understand Docker image and container
	首先是确保Docker打开，我用的是Linux 直接在TERMIMAL上设置
        （需要能熟练使用linux命令如： ls/cd/copy等， 还需要注意路径）
	第一个掌握command: build
	第二个掌握command: run （可以加 rm）---测试网站是否能在本地使用
	第三个掌握command: stop
	需要注意：container名字叫 webapp_1
	dockerfile: 需要会读和写，理解
	可以在docker hub上找相关信息: 比如查alpine

	Docker file 例子：
```
FROM python:3

# set a directory for the app
WORKDIR /usr/src/app

# copy all the files to the container
COPY . .

# install dependencies
RUN pip install --no-cache-dir -r ./src/requirements.txt

# define the port number the container should expose
EXPOSE 5000

# run the command
CMD ["python", "./src/app.py"]
```

   Flask (Python framework)
   http: default port 80
   https: default port 443
   you can use ports after 1024 like port 5000 or  port 5001


app.py




## 4 practices for docker file:


#1. console-helloworld
#2. web-nginx
#3. web-python-flask
#4. console-dependency
