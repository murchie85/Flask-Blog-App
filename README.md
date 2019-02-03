# FLASK BLOGGING APPLICATION 

![FLASK IMAGE](https://cdn-images-1.medium.com/max/438/1*0G5zu7CnXdMT9pGbYUTQLQ.png)

## DEPENDENCIES
Using Anaconda with virtual env

- Python 3
- Flask

## Running a simple web page 

Getting started with a simple flask application: 

1. Create a directory FLASK_BLOG
2. `cd FLASK_BLOG`
3. Set up a virtual environment (download anaconda) then create your environment to work in 
4. `pip install flask`
5. Create a file called `flaskblog.py`

Now lets start adding code to `flaskblog.py` , you can go to the flask main website which gives you your first hello world code to work with [here](http://flask.pocoo.org/) or just copy and paste the code below: 

```
from flask import Flask
app = Flask(__name__)


@app.route("/")
def hello():
	return "Greetings bloggers"

```


Before you run application we need to set an environment variable.

For Mac: 

```
export FLASK_APP=flaskblog.py
````
In windows the command is set (I think). Then we can run the app simply by executing: 

```
flask run
```

Ensure you are in the FLASK_BLOG directory, and if all works ok check localhost:5000
