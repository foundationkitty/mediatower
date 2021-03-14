FROM linuxserver/ffmpeg

RUN apt update && apt dist-upgrade -y && apt install python3-pip -y && pip3 install locast2dvr

EXPOSE 5000

ENTRYPOINT ["locast2dvr","--config","/config/config"]
