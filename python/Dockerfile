FROM python:stretch

RUN mkdir /opt/server
WORKDIR /opt/server

COPY requirements.txt requirements.txt
RUN pip3 install -r requirements.txt

COPY server.py server.py
EXPOSE 5000

ENTRYPOINT ["python3"]

CMD ["server.py"]
