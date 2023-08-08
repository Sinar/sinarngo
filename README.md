# Sinar NGO

## Installation and Buildout

### Ubuntu 22.04 LTS

Setup system dependencies:

```
sudo apt install build-essential python3-dev
```

Setup venv and buildout environment:

```
python3.8 -m venv venv
venv/bin/pip install setuptools zc.buildout==3.0.1 wheel==0.38.4 \
plonecli
venv/bin/buildout bootstrap
```

Run buildout:

```
bin/buildout -vvv
```

Starting service in foreground debug mode:

```
bin/instance fg
```
