FROM debian:stable-slim
LABEL date=26022021
RUN sudo apt-get install python3-picamera
RUN sudo apt-get install python3-pip
RUN sudo pip3 install ws4py
RUN sudo apt-get install ffmpeg

WORKDIR /app
RUN git clone https://github.com/waveform80/pistreaming.git ./
CMD ["python3 ", "server.py"]

# docker-compose up --build