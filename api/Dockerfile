FROM python:3.6
LABEL maintainer vincentinttsh
ENV PYTHONUNBUFFERED 1
RUN mkdir /run_data
RUN mkdir /api_data
WORKDIR /api_data
COPY ./code /api_data
RUN pip install -r requirements.txt
RUN base64 /dev/urandom | head -c50 > secretkey.txt
