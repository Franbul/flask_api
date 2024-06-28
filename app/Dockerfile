# Dockerfile
FROM python:3.10-slim

WORKDIR /app

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt
RUN pip install uwsgi uwsgitop  # Ensure uwsgi and uwsgitop are installed

COPY . .

CMD ["uwsgi", "--ini", "uwsgi.ini"]
