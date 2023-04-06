FROM python:3.10-alpine

ENV LANG C.UTF-8 \
    TZ 'Asia/Shanghai' 

WORKDIR /app

ADD jdsign/jdsign.py .
ADD https://github.com/walle1798/WALL.E/raw/master/signapi.py .

Run pip install flask \
    && apk add --no-cache tzdata && \
    ln -sf /usr/share/zoneinfo/$TZ /etc/localtime && \
    echo $TZ > /etc/timezone 

ENTRYPOINT ["python", "signapi.py"]