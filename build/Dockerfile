FROM ubuntu:hirsute AS btc-build
RUN apt-get update && apt-get upgrade -y
LABEL date=26022021
RUN apt-get install python3-picamera
RUN apt-get install python3-pip
RUN pip3 install ws4py
RUN apt-get install ffmpeg

WORKDIR /app
RUN git clone https://github.com/waveform80/pistreaming.git ./
CMD ["python3 ", "server.py"]

# docker-compose up --build