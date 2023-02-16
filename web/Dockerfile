FROM python:3.7

COPY . /
RUN pip install -r requirements.txt
RUN pip install gunicorn
ENV FLASK_APP /app/server.py

CMD gunicorn --bind 0.0.0.0:8000 app.app:app

EXPOSE 8000
