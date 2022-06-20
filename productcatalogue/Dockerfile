FROM openjdk:8-jre
ADD /home/bandaru/kubernetes-yamls/myagent/_work/1/a/productcatalogue/target/productcatalogue-0.0.1-SNAPSHOT.jar app.jar
ADD product-catalogue.yml app-config.yml
EXPOSE 8020
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","app.jar", "server", "app-config.yml"]
