# Python PIP Skeleton

## Execute

One of the following:

```
$ bin/hello
$ python -m hello
$ python hello/__main__.py
```

## Install

One of the following:

```
$ pip install -e Hello
$ python setup.py install
```

## Develop

Main: `hello/__init__.py`

Logic: `hello/Hello.py`

## Publish to PyPI

Strongly suggest to read over [Uploading your Project to PyPI](http://python-packaging-user-guide.readthedocs.org/en/latest/distributing/#uploading-your-project-to-pypi)

### Requeriments

Python 2: `apt-get install python-setuptools`

Python 3: `apt-get install python3-setuptools`

### First time

```
$ python setup.py register
```
Beware that passwords are sent plain text. See [twine](https://packaging.python.org/en/latest/projects/#twine)

### Recurrent
```
$ python setup.py upload
```
Beware that passwords are sent plain text. See [twine](https://packaging.python.org/en/latest/projects/#twine)

### Pypi config file

Edit: `~/.pypirc`

```
[distutils]
index-servers=pypi

[pypi]
repository=https://pypi.python.org/pypi
username=<username>
password=<password>
```
