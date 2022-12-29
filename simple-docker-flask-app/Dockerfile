FROM python:3.8

# set work directory for app
WORKDIR /usr/src/app

# copy all the files to container
COPY . .

RUN pip install --no-cache-dir -r requirements.txt

# Expose application/container port number
EXPOSE 5000

# run the command for executing the flask app script
CMD ["python", "./app.py"]
