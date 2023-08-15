WORKDIR /project/registro

COPY . .

RUN pip install --upgrade pip
RUN pip install django
RUN pip install djangorestframework


EXPOSE 8000

CMD ["python", "manage.py", "runserver", "127.0.0.1:8000"]
