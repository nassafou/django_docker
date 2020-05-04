FROM python:3.4
MAINTAINER Yoz

COPY ./app /app

WORKDIR /app
RUN pip install Django
RUN pip install psycopg2
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
