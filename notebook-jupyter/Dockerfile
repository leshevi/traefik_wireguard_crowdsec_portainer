FROM python:slim

WORKDIR /app

RUN apt-get update && apt-get install -y \

    gcc \
    python3-dev \
    musl-dev \
    linux-header-* \
    python3-psutil;

RUN pip install --no-cache psutil notebook;

EXPOSE 8888

CMD ["jupyter", "notebook", "--ip=0.0.0.0", "--port=8888", "--no-browser", "--allow-root"]
