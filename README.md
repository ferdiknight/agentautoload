# agentautoload
An example of java9+ Launcher-Agent-Class attribute.

build the project,and you can find a tar.gz file and a dir both named agent-autoload
```shell
mvn clean package 
```
go into the agent-autoload dir, run 
```shell
java -jar agent-autoload.jar
```
if you run this with jdk9 or higher, you will get output like this:
```shell
=================agent loaded=================
test
```
and if you run this with jdk8 or lower, you just get only test :
```shell
test
```
because the Launcher-Agent-Class is added since jdk9, so it won`t work on jdk8 or lower.
