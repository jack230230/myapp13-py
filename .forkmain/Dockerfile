FROM python:3.10

WORKDIR /workdir

COPY ./ ./

RUN pip3 install -r requirements.txt

EXPOSE 5000

CMD ["sh", "-c", "gunicorn --workers=2 -b 0.0.0.0:5000 app:app"]
