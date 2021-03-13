# python-bottle

## Install bottle
```
pip install bottle
```

create a virtualenv first:
```
$ virtualenv develop                # Create virtual environment
$ source develop/bin/activate       # Change default python to virtual one
(develop)$ pip install -U bottle    # Install bottle to virtual environment
```

## Application
create `main.py`
```
from bottle import route, run

@route('/hello')
def hello():
    return "Hello World!"

run(host='localhost', port=8080, debug=True)
```

## Run App
```
(develop) $ python main.py
```

source: https://bottlepy.org/docs/dev/tutorial.html