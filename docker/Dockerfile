FROM ubuntu
MAINTAINER vladov

RUN echo "0.1" > /version

VOLUME /minecraftServer

RUN apt-get update
RUN apt-get -y install wget
RUN apt-get -y install tmux
RUN apt-get -y install bzip2
RUN apt-get -y install openjdk-8-jre
RUN wget https://s3.amazonaws.com/Minecraft.Download/versions/1.10.2/minecraft_server.1.10.2.jar
RUN mv /minecraft_server.1.10.2.jar /minecraftServer/minecraft_server.jar
EXPOSE 25565
