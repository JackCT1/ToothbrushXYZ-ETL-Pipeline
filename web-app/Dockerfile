FROM python:3.10
ENV APP_HOME /app
WORKDIR $APP_HOME


ADD requirements.txt ./
RUN pip3 install -r requirements.txt

COPY . .

ENV PYTHONUNBUFFERED True

CMD python3 app.py