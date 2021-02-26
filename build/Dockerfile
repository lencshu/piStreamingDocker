FROM python:3.8-slim
LABEL date=26022021

RUN apt-get install ffmpeg

RUN pip install --no-cache-dir ws4py
RUN pip install --no-cache-dir picamera

WORKDIR /app
RUN git clone https://github.com/waveform80/pistreaming.git ./
CMD ["python3 ", "server.py"]

# docker-compose up --build