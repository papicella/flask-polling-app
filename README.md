# flask-polling-app
A simple web polling application written in Python (Flask).

![flask_image1](https://user-images.githubusercontent.com/25560159/201449980-f18fcbe8-320d-41ed-97a4-6cf8431033dd.png)
![flask_image2](https://user-images.githubusercontent.com/25560159/201450001-5e2c2eeb-06af-4dfa-8cc3-5d9c27d2a118.png)

## Deployment
Python version:
```
python --version
Python 3.6.15
```

Install the dependencies:

```
pip install -r requirements.txt
```

and start the application:

```
python app.py
Check if a poll already exists in the db
...
* Running on http://0.0.0.0:8080/ (Press CTRL+C to quit)
```

## Docker build and deployment

Build a Docker image:

```
docker build -t flask-polling-app:latest .
``` 

Start the container:

```
docker run -d -p 8080:8080 --name=flask-polling-app flask-polling-app:latest
```
