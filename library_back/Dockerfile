FROM python:3.9.5-slim-buster

WORKDIR /app

COPY requirements.txt /app/

RUN apt-get update \
    && apt-get -y install libpq-dev gcc
  
RUN pip3 install -r requirements.txt

COPY . .

# RUN python manage.py makemigrations \
#     && python manage.py migrate

# CMD ["python", "manage.py", "runserver"]