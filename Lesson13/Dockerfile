FROM python:3.9.5-buster

ENV PYTHONUNBUFFERED=1

WORKDIR /app

COPY requirements.txt ./requirements.txt
RUN pip install -r requirements.txt

COPY ../../../Downloads/Origin-master/lesson%2013 .
CMD gunicorn main:app --access-logfile '-' --bind 0.0.0.0:8000