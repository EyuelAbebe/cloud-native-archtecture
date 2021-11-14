FROM python:2.7

WORKDIR /home

ADD . /home

RUN pip install --no-cache-dir -r requirements.txt

EXPOSE 3111

CMD ["python", "init_db.py"]

ENTRYPOINT FLASK_APP=/home/app.py flask run --host=0.0.0.0 --port=3111