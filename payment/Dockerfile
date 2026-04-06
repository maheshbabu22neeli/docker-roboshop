FROM python:3.9

WORKDIR /app

EXPOSE 8080

COPY requirements.txt .
COPY *.py .
COPY payment.ini .

RUN pip3 install -r requirements.txt

CMD ["uwsgi", "--ini", "payment.ini"]