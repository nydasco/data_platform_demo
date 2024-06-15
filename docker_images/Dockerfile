FROM openjdk:19-buster

ENV MB_PLUGINS_DIR=/home/plugins/

ADD https://downloads.metabase.com/v0.46.2/metabase.jar /home
ADD https://github.com/Baoqi/metabase-dremio-driver/releases/download/1.3.1/dremio.metabase-driver.jar /home/plugins/

RUN chmod 744 /home/plugins/dremio.metabase-driver.jar

CMD ["java", "-jar", "/home/metabase.jar"]