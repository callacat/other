FROM python:3.10-alpine

ENV LANG C.UTF-8 \
    TZ 'Asia/Shanghai' 

WORKDIR /app

ADD jdsign/jdsign.py .
ADD https://github.com/walle1798/WALL.E/raw/master/signapi.py .

ENTRYPOINT ["python", "signapi.py"]