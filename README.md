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


Before you run application we need to set an environment variable in terminal or command line.

For Mac: 

```
export FLASK_APP=flaskblog.py
````
In windows the command is set *(I think)*. Then we can run the app simply by executing: 

```
flask run
```

Ensure you are in the FLASK_BLOG directory, and if all works ok put `localhost:5000` into your browser and you should see the message 'greetings bloggers'.


## WHAT JUST HAPPENED? 

When you executed `flask run` what happened was the flask framework looked at the environment variable we set `FLASK_APP` then started running the python application that you called 'flaskblog.py'. It runs this on your computer, until you stop the process by pressing the following: 

```
ctl + c
```

This terminates the process, but bare in mind what just happened was we run an application on our flask server. We were effectively serving content (our greeting  message) which we could in theory serve externally to the public.


## REFINEMENTS

Lets make it look nicer by changing the message `"Greetings bloggers"` to `"<h1>Greetings bloggers<\h1>"` this is html header tags, if you don't know what this is, it is the markup code which formats how text and images are displayed in a web browser. It is standard must know knowledge for any web developer or coder in general and rather easy to learn in short time.

Make sure you stop your webserver with `ctl + c` on the command line  / terminal and start it again with `flask run`
