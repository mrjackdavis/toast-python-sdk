# Toast Python SDK

# Deploying to PyPi

Python package management is 100% crazy. I've had to do this by launching a python docker image interactively using `bash` as the command

    docker run --name=toast-python-sdk  -i -t python:3.4.3 /bin/bash

Then, I had to `pip install twine`, setup a [~/.pypirc](https://packaging.python.org/en/latest/distributing.html#register-your-project) file, `python setup.py sdist` then `twine upload dist/*`. Crazy pants.

