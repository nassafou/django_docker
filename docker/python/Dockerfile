FROM python:3.4
MAINTAINER Yoz

COPY ./app /app

WORKDIR /app
RUN pip install Django
RUN pip install psycopg2

COPY ./docker/python/entrypoint.sh /entrypoint.sh

RUN chmod +x /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]

#CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
