FROM python:3.9-slim

ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ENV CONTAINERENV True

ADD templates/index.html templates/index.html
ADD name.txt name.txt
ADD mail.txt mail.txt

ADD app.py app.py
ENTRYPOINT python3 app.py