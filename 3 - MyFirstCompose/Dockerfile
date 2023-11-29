FROM ubuntu

RUN apt-get update --fix-missing -y
RUN apt-get install pip -y
RUN pip install flask

WORKDIR /app
COPY . /app

RUN pip --no-cache-dir install -r requirements.txt

CMD ["python3", "app.py"]