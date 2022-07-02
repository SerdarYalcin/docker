FROM ubuntu

RUN apt-get update && apt-get install -y python2 python-pip
RUN pip2 install flask

COPY app.py /opt/
CMD sleep 10

ENTRYPOINT FLASK_APP=/opt/app.py flask run --host=0.0.0.0 --port=8080
