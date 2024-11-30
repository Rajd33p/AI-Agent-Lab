FROM python:3.9
ENV PYTHONUNBUFFERED 1
WORKDIR /app
RUN apt-get update
RUN apt-get install -y sqlite3 build-essential
COPY docker-requirements.txt /app/
RUN pip install --no-cache-dir -r docker-requirements.txt
COPY . /app/
