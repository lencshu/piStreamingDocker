FROM ubuntu:xenial
RUN apt-get update && apt-get upgrade -y
LABEL date=26022021
RUN apt-get install python3-pip -y
RUN apt-get install python3-picamera -y
RUN pip3 install ws4py -y
RUN apt-get install ffmpeg -y

WORKDIR /app
RUN git clone https://github.com/waveform80/pistreaming.git ./
CMD ["python3 ", "server.py"]

# docker-compose up --build