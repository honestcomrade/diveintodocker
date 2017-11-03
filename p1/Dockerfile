FROM python:2.7-alpine

RUN mkdir /app
WORKDIR /app

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

COPY . .

LABEL maintainer="Joe Saraceno <honestcomrade@gmail.com>" \
      version="0.9"

CMD flask run --host=0.0.0.0 --port=5000