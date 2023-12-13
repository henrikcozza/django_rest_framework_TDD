# pull official base image
FROM python:3.11.2-slim-buster

# set working directory
WORKDIR /user/src/app

# set environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

# install dependences
RUN pip install --upgrade pip
COPY ./requirements.txt .
RUN pip install -r requirements.txt

# include the app
COPY . .