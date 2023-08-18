FROM python:3.9

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

WORKDIR /project/registro

COPY . .

RUN pip install --upgrade pip
RUN pip install django
RUN pip install djangorestframework


EXPOSE 8000

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
