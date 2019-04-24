FROM python:3

WORKDIR /usr/src/app

COPY requirements.txt ./

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
        build-essential \
        vim \
    && pip3 install --upgrade pip \
    && pip install --no-cache-dir -r requirements.txt


