FROM python:3.9.1-slim-buster

WORKDIR /app

COPY app.py /app

RUN pip install flask

EXPOSE 5000
CMD ["python", "app.py"]