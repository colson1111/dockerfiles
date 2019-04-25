FROM python:3-slim

LABEL maintainer="Craig Olson <colson1111@gmail.com>"

COPY requirements.txt .

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
        build-essential \
        vim \
    && pip3 install --upgrade pip \
    && pip3 install --no-cache-dir -r requirements.txt \
    && rm -rf $HOME/.cache \
    && apt-get purge -y python.* \
    && apt-get autoremove -y \
    && apt-get clean

CMD ["/bin/bash"]
