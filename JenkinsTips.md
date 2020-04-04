Jenkins Tips
========



#### Jenkinsfile 

Jenkinsfile 可以构建比较好看的pipline job，可以把jenkinsfile 放在GitHub，然后每次去拿这个文件，执行命令



#### Jenkins 和 GitHub 联合认证

Jenkins可以和GitHub联合认证，然后在GitHub上申请的secret或者说token，可以在jenkins-cli里当password用

（token sample：42a6efec86514bed6202d78a1891a317dxxxxxx ）

<img src="img\01GitHub设置accessToken1.png" style="zoom:50%;" />

<img src="img\02GitHub设置accessToken2.png" style="zoom:50%;" />



##### 用jenkins-cli.jar触发job的例子：

java -jar jenkins-cli.jar -s http://\<FQDN\>:8080 -auth name:token build \<Job full name\> -v -s

注意：这个jar工具的命令参数好像有一定的顺序要求，顺序不对，执行不了








