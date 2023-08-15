FROM python:3.8

# Create a non-root user and switch to it
RUN useradd -ms /bin/bash myuser
USER myuser

WORKDIR /project/registro

COPY --chown=myuser . .

RUN pip install --upgrade pip && \
    pip install django djangorestframework

EXPOSE 8000

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
