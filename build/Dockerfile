FROM plexcloudmusic/ffmpeg
LABEL date=26022021

RUN pip3 install --no-cache-dir ws4py
RUN pip3 install --no-cache-dir picamera

WORKDIR /app
RUN git clone https://github.com/waveform80/pistreaming.git ./
CMD ["python3 ", "server.py"]

# docker-compose up --build