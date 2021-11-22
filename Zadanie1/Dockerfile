#okreslamy obraz podstawowy
FROM python:3.10.0-alpine3.14

MAINTAINER Mr. Vladyslav Havryliuk

#opisujemy metadane
LABEL version="1.0"

#zmienna srodowiskowa portu
ENV PORT="7000"

#kopijujemy plik programu do kontenera
COPY web_app.py /

#tworzymy port
EXPOSE ${PORT}

#instalujemy biblioteki
RUN pip install requests && pip install pytz

#uruchomienie skryptu 
CMD python -u web_app.py
