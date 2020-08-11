FROM java:8-jre
ADD  ./Mycat-server.tar.gz /opt

VOLUME /opt/mycat/conf
EXPOSE 8066 9066
ENV MYCAT_HOME=/opt/mycat/
ENV PATH=$PATH:$MYCAT_HOME/bin
WORKDIR $MYCAT_HOME/bin
RUN chmod u+x ./mycat
CMD ["./mycat", "console"]

