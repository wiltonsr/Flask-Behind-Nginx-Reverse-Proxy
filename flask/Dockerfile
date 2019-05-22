FROM python:3.7.2-alpine

ENV FLASK_APP app.py

ADD ./requirements.txt /config/

RUN pip install --upgrade pip

RUN pip install -r /config/requirements.txt

ADD /app /app

WORKDIR /app

ENTRYPOINT ["flask", "run", "--host=0.0.0.0"]
