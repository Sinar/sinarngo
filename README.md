# Sinar NGO

A Plone buildout for Plone site with common add-ons and behaviours for 
a unified NGO website for public publication of content and capturing MEL metadata.

Currently in use by:

 * Sinar Project website https://github.com/Sinar/sinarproject.org
 * Enabling Tech website https://github.com/Sinar/enabling-tech
 * Intranet https://github.com/Sinar/foe-km/
 * Public Project site (iMAP) https://github.com/Sinar/imap
   

## Installation and Buildout

### Ubuntu 24.04 LTS

#### Setup system dependencies:

```
sudo apt install build-essential python3-dev python3-venv
```

#### Setup venv and buildout environment U

```
python3 -m venv venv
venv/bin/pip install setuptools==75.8.2 zc.buildout==4.1.3 wheel==0.45.1 \
plonecli
venv/bin/buildout bootstrap
```

### Buildout

Run buildout:

```
bin/buildout -vvv
```

Starting service in foreground debug mode:

```
bin/instance fg
```
