FROM openjdk:8-jdk-alpine

VOLUME /tmp

# ADD 拷贝文件明并重命名
ADD ./dubbo-admin-server-0.2.0-SNAPSHOT.jar app.jar

# ENTRYPOINT,为了缩短Tomcat的启动时间,添加 java.security.egd的系统属性指向/dev/urandom 作为ENTRYPOINT
ENTRYPOINT [ "java", "-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]
