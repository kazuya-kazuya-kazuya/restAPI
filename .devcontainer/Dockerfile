FROM python:3.11-slim


# Linuxツール
RUN apt-get update && apt-get install -y \
    git \
    curl \
    vim \
    build-essential \
    && rm -rf /var/lib/apt/lists/*


# 作業場所
WORKDIR /workspaces/restAPI


# Pythonライブラリ
COPY requirements.txt /tmp/requirements.txt

RUN pip install --upgrade pip \
    && pip install -r /tmp/requirements.txt


CMD ["sleep", "infinity"]