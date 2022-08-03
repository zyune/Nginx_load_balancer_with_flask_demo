FROM python:3.9-slim

WORKDIR /app

COPY . .

RUN pip install -r requirement.txt

CMD gunicorn --bind 0.0.0.0:5000 server1:app