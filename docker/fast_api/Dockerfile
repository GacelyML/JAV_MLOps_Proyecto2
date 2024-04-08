FROM python:3.10-slim-buster
# Install python packages
COPY ./requirements.txt /tmp/requirements.txt
RUN pip install -r /tmp/requirements.txt
RUN python -m pip install mlflow
