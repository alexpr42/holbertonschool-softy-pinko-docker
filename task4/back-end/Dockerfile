FROM ubuntu:latest

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && apt-get install -y python3 python3-pip python3-venv

RUN python3 -m venv /venv

RUN /venv/bin/pip install --upgrade pip

RUN /venv/bin/pip install flask flask-cors

WORKDIR /app

COPY ./api.py /app/api.py

CMD ["/venv/bin/python", "/app/api.py"]
