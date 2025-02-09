FROM python:3.10.16-alpine3.21

COPY . /app

WORKDIR /app

COPY ./requirements.txt ./

RUN pip install -r requirements.txt

RUN python manage.py migrate

CMD ["python","manage.py","runserver","0.0.0.0:8000"]