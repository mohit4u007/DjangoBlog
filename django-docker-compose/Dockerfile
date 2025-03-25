# FROM python:3.9.5-alpine

RUN mkdir /app
WORKDIR /app

# Set environment variables to optimize the Python runtime
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

RUN pip install --upgrade pip
COPY ./requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY ./django_project .

COPY ./entrypoint.sh .
ENTRYPOINT ["sh", "entrypoint.sh"]