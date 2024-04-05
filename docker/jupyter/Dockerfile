FROM python:3.9
ARG MLFLOW_S3_ENDPOINT_URL=http://minio:8081
ARG AWS_ACCESS_KEY_ID=supersecretaccess2024
ARG AWS_SECRET_ACCESS_KEY=supersecretaccess2024
RUN mkdir /work
COPY ./requirements.txt /tmp/requirements.txt
RUN pip install jupyter==1.0.0 -U && pip install jupyterlab==3.6.1
RUN pip install -r requirements.txt