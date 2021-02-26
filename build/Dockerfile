FROM plexcloudmusic/ffmpeg
LABEL date=26022021

RUN pip3 install ws4py
RUN pip3 install picamera

WORKDIR /app
RUN git clone https://github.com/waveform80/pistreaming.git ./
CMD ["python3 ", "server.py"]

# docker-compose up --build