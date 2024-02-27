# Dockerfile in the root directory
FROM python:3.9

WORKDIR /app

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

COPY app.py .
COPY ./templates .
COPY ./static .

CMD ["python", "app.py"]

