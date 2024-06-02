FROM python:3.11
WORKDIR /code

COPY ./requirements.txt /code/requirements.txt
COPY ./app /code/app

RUN apt-get update
RUN pip install --no-cache-dir --upgrade -r /code/requirements.txt
CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "80"]
