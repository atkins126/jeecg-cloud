FROM anapsix/alpine-java:8_server-jre_unlimited

MAINTAINER jeecgos@163.com

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

RUN mkdir -p /jeecg-cloud-demo-biz

WORKDIR /jeecg-cloud-demo-biz

EXPOSE 8002

ADD ./target/jeecg-cloud-demo-biz-2.2.0.jar ./

CMD java -Djava.security.egd=file:/dev/./urandom -jar jeecg-cloud-demo-biz-2.2.0.jar
