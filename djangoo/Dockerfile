# Dockerfile
FROM python:3.8

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

WORKDIR /code/djangoo

COPY requirements.txt /code/djangoo/
RUN pip install -r requirements.txt

COPY . /code/djangoo/

EXPOSE 8000

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]