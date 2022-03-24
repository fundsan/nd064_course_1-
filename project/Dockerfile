## Docker commands used to build the application 
FROM python:2.7
LABEL maintainer="Jake Fund"
COPY ./techtrends /app

WORKDIR /app
RUN pip install -r requirements.txt

RUN python init_db.py
EXPOSE 3111
CMD [ "python", "app.py" ]