# JHipster文档环境搭建 （此文采用Markdown语法编写）

* JHipster官方文档：https://www.jhipster.tech/

## 背景环境  
* node:8.12.0（当前稳定版）
  ### 安装方法  
    * 【系统变量】下新建【NODE_PATH】  
        C:\Program Files\nodejs\node_modules  

    * 【用户变量】下的【Path】  
        C:\Program Files\nodejs  

    * node -v  

* yarn 
  ### 安装方法  
    * ```npm install -g yarn```
* JDK8  
  ### 安装方法  
    * 系统变量→新建 JAVA_HOME 变量  
      变量值填写jdk的安装目录（本人是 C:\Program Files\Java\jdk1.8.0_181)
  
    * 系统变量→寻找 Path 变量→编辑  
      %JAVA_HOME%\bin;%JAVA_HOME%\jre\bin;
  
    * 系统变量→新建 CLASSPATH 变量  
      .;%JAVA_HOME%\lib;%JAVA_HOME%\lib\tools.jar
  
    * 运行cmd 输入 java -version   
* mysql （笔者是使用mysql） 
  ### 安装方法  
  * 新建MYSQL_HOME变量  
    D:\soft\mysql-5.7.23-winx64
  
  * 编辑path系统变量  
    %MYSQL_HOME%\bin
### 推荐安装  
* git  
* IDEA （有破解方法）  
  ### 破解方法  
    * host文件位置：C:\Windows\System32\drivers\etc  
      请将“0.0.0.0 account.jetbrains.com”添加到hosts文件中  
    * http://idea.lanyus.com/  
      获取注册码；填写idea注册
* Navicat Premium （破解补丁）  
  ### 破解方法  
    * 安装navicat12018_premium_cs_x64  

    * Navicat Premium 12 破解补丁  

    * 把补丁包内对应版文件拷贝到navicat12018_premium_cs_x64安装目录下  

## 安装jhipster
* 安装jhipster:```npm install -g generator-jhipster```   
* 新建项目文件：```mkdir testjhipster```  
* 进入此文件： ```cd testjhipster```
* 执行命令： ```jhipster```

## 项目运行
* 运行指令： ```./mvnw或者mvnw```运行
* 运行会报错：
   * 修改yml数据库地址
   * 构建项目前端部分：
     * ```yarn```
     * ```yarn add node-sass```
     * ```yarn start```
     * 重新```./mvnw或mvnw```启动项目


## 项目运行控制中心: http://localhost:8080

---------------------------------------

作者：``Vinci LoveEmperor``