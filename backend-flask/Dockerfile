FROM python:3.10-slim-buster

#Inside the Container
#Make a new folder inside the container
WORKDIR /backend-flask

#Outside the Container -> Inside the Container
COPY requirements.txt requirements.txt
RUN pip3 install -r requirements.txt

COPY . .

#Set Environment Variables
#Inside Container and will remain set while the container is running
ENV FLASK_ENV=development
#python -m flask run --host=0.0.0.0 --port=4567
EXPOSE ${PORT}
CMD ["python3", "-m", "flask", "run", "host=0.0.0.0", "--port=4567"]