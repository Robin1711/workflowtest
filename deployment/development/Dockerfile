# Dockerfile has to be execute in the root dir
FROM python:3.11

ENV PYTHONUNBUFFERED=1

WORKDIR /app

COPY src/requirements.txt /app

RUN pip install --no-cache-dir -r requirements.txt

COPY src/ /app

EXPOSE 8000

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
