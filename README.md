# Flask-FontAwesome
[![PyPI Version](https://badge.fury.io/py/Flask-FontAwesome.svg)](https://pypi.python.org/pypi/Flask-FontAwesome) [![CI](https://api.travis-ci.org/heartsucker/flask-fontawesome.svg?branch=develop)](https://api.travis-ci.org/heartsucker/flask-fontawesome.svg?branch=develop) [![Documentation Status](https://readthedocs.org/projects/flask-fontawesome/badge/?version=latest)](https://flask-fontawesome.readthedocs.io/en/latest/?badge=latest)

Dowload for Taho: `pip install --upgrade git+https://github.com/Taho-DiscordBot/flask-fontawesome.git`

Flask extension for [FontAwesome](https://fontawesome.com/).

## Example

```python
from flask import Flask, render_template
from flask_fontawesome import FontAwesome

app = Flask(__name__)
fa = FontAwesome(app)

@app.route('/')
def index():
    return render_template('index.html')

app.run(host='127.0.0.1', port=8080)
```

```html
<!DOCTYPE html>
<html>
  <head>
    {{ fontawesome_html() }}
    <title>FontAwesome Example</title>
  </head>
  <body>
    <h1>FontAwesome Example</h1>
    <p>This is an example of a <span class="fas fa-link"></span> link.</p>
  </body>
</html>
```

## License

This work is dual licensed under the MIT and Apache-2.0 licenses. See [LICENSE-MIT](./LICENSE-MIT)
and [LICENSE-APACHE](./LICENSE-APACHE) for details.

### Attribution

The resources contained under [`flask_fontawesome/static`](./flask_fontawesome/static) are licensed to FontAwesome.
