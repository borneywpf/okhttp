# 官方实例调试方法

## 编译okhttp
> mvn install(mvn compile)

通过编译会在相应的module目录的target目录下生成jar包，我们用到okhttp/target/okhttp-3.4.2-SNAPSHOT.jar

## 实例调试

> 
1.先将代码GetExample拷贝到src目录下  
2.将编译生成的jar包(上述的okhttp-3.4.2-SNAPSHOT.jar)拷贝的lib目录下  
3.因为运行okhttp需要使用okio，所以需要将okio的jar包也拷贝的lib目录下  
4.编译实例代码
 + 在aread-okhhtp目录下运行命令： **javac -cp .:./lib/* src/GetExample.java**  
> 
5.运行实例代码
 + 通过第四步的编译会生成一个GetExample.class文件，通过命令行运行: **java -cp .:lib/*:src GetExample**  

可以通过同样的方式调试PostExample.java
