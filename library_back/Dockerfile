FROM python:3.9.5-slim-buster

WORKDIR /app

COPY requirements.txt /app/

COPY . .

RUN apt-get update \
    && apt-get -y install libpq-dev gcc

RUN pip3 install gunicorn

RUN pip3 install -r requirements.txt

RUN chmod +x ./setup_env.sh && ./setup_env.sh
