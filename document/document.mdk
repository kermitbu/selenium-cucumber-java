Title         : Cucumber+Java
Author        : Kermit
Logo          : True

[TITLE]

# 环境配置 

- Maven下载地址：

[http://maven.apache.org/download.cgi](http://maven.apache.org/download.cgi)


- JDK下载地址：

[https://www.oracle.com/technetwork/java/javase/downloads/index-jsp-138363.html](https://www.oracle.com/technetwork/java/javase/downloads/index-jsp-138363.html)

JDK最好下载1.8版本，高版本会有警告.

下载完成之后，安装。
之后配置环境变量。

```
JAVA_HOME=JDK的安装路径
MAVEN_HOME=MAVEN的安装路径
Path中增加%MAVEN_HOME%/bin;%JAVA_HOME%/bin;
```

修改%MAVEN_HOME%/conf/settings.xml中的mirrors标签,像下面这样增加镜像路径

```
<mirrors>
    <!-- mirror
     | Specifies a repository mirror site to use instead of a given repository. The repository that
     | this mirror serves has an ID that matches the mirrorOf element of this mirror. IDs are used
     | for inheritance and direct lookup purposes, and must be unique across the set of mirrors.
     |
    <mirror>
      <id>mirrorId</id>
      <mirrorOf>repositoryId</mirrorOf>
      <name>Human Readable Name for this Mirror.</name>
      <url>http://my.repository.com/repo/path</url>
    </mirror>
     -->
    <mirror>
        <id>alimaven</id>
        <mirrorOf>central</mirrorOf>
        <name>aliyun maven</name>
        <url>http://maven.aliyun.com/nexus/content/repositories/central/</url>
    </mirror>
    <mirror>
        <id>jboss-public-repository-group</id>
        <mirrorOf>central</mirrorOf>
        <name>JBoss Public Repository Group</name>
        <url>http://repository.jboss.org/nexus/content/groups/public</url>
    </mirror>
</mirrors>
```
# 创建项目

1. 创建一个文件夹存放文件
2. 进入文件夹，CMD执行如下命令 (下面是Cucumber官网给出的创建工程的Demo, 可根据实际情况调整参数)

```
  mvn archetype:generate -DarchetypeGroupId=io.cucumber -DarchetypeArtifactId=cucumber-archetype -DarchetypeVersion=2.3.1.2 -DgroupId=hellocucumber -DartifactId=hellocucumber -Dpackage=hellocucumber -Dversion=1.0.0-SNAPSHOT -DinteractiveMode=false
  

3. 按照[https://docs.cucumber.io/guides/10-minute-tutorial/](https://docs.cucumber.io/guides/10-minute-tutorial/)中的说明修改对应文件。
4. 在项目目录中[demo的目录是hellocucumber]执行 mvn test 

# 引入Selenium
