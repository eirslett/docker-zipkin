FROM openzipkin/zipkin-base:1.2.2
MAINTAINER OpenZipkin "http://zipkin.io/"

RUN curl -SL $ZIPKIN_REPO/io/zipkin/zipkin-query-service/$ZIPKIN_VERSION/zipkin-query-service-$ZIPKIN_VERSION-all.jar > zipkin-query.jar

ADD run.sh /usr/local/bin/run.sh
ENTRYPOINT ["/usr/local/bin/run.sh"]

EXPOSE 9411
