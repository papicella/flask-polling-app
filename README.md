# flask-polling-app
A simple web polling application written in Python (Flask).

## Deployment

Install the dependencies:

```
pip3 install flask
pip3 install flask-sqlalchemy
pip3 install mysqlclient
```

and start the application:

```
python3 app.py
Check if a poll already exists in the db
...
* Running on http://0.0.0.0:8080/ (Press CTRL+C to quit)
```

## Docker build and deployment

Build a Docker image:

```
docker build -t polling-app:latest .

Start the container:

```
docker run -d -p 8080:8080 --name=polling-app polling-app:latest
```