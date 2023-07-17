# syntax=docker/dockerfile:1.4

FROM python:3.7-alpine
EXPOSE 8000
WORKDIR /djsite
COPY requirements.txt /djsite
RUN pip3 install -r requirements.txt --no-cache-dir
COPY . /djsite
ENTRYPOINT ["python3"]
CMD ["manage.py", "runserver", "0.0.0.0:8000"]
