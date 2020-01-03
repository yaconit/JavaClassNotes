# 什么是Maven
maven是一个jar包的仓库，里面放置了各种各样的jar包，这些jar包使用pom.xml文件进行管理

# 为什么要用Maven
- 统一通过pom.xml进行引用
- 无须手动导入jar文件
- 方便项目移植
- 适合多人开发

# maven命令
- clean ==> 清空上一次项目运行生成的文件
- package ==> 下载构建并打包项目
> 打包的结果受`<packaging>jar</packaging>`配置影响

# 在项目中导入jar包
在pom.xml文件中添加以下代码：
```xml
<dependencies>
    <dependency>
        <groupId>...</groupId>
        <artifactId>...</artifactId>
        <version>...</version>
    </dependency>
</dependencies>
```

# maven注意点
1. 类必须都要从属于某一个包中，否则，后期无法进行引用
2. 依赖都有传导性

# 为什么要把正项目拆分
1. 开发人员不是一个人
2. 某个模块运行压力过大

# 如何拆项目
1. 把访问量大的某块拆出来
2. 把公共模块拆出来
3. 把需要单独维护的模块拆出来
4. 根据开发人员进行模块拆分