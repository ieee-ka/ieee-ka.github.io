# Website of the IEEE Student Branch Karlsruhe

This repository contains the sources of our website. It is build using the static site generator [Nikola](https://getnikola.com/). And deployed to the branch gh-pages and available on http://ieee-ka.de

### Build

1. To build we use [Conda](http://conda.pydata.org/) to create the build environment:
```sh
$ git clone https://github.com/ieee-ka/ieee-ka.github.io  # or the URL to your fork
$ cd ieee-ka.github.io  # the repo base directory
$ conda env create
$ source activate nikola
$ nikola build
```
With this setup the site can be edited, build and deployed using the ```nikola``` command

OR

2. Create python virutal environment and install with requirements (project currently only with python3.9):
```sh
$ git clone https://github.com/ieee-ka/ieee-ka.github.io  # or the URL to your fork
$ cd ieee-ka.github.io  # the repo base directory
$ python3 -m venv nikolaenv
$ source nikolaenv/bin/activate
$ pip install -r requirements.txt
$ nikola build
```

### View

View changes in newly opened browser
```sh
$ nikola serve -b
```

### Update

To update your build envirement you can use:
```sh
$ conda update conda  # optional
$ cd ieeekasite  # the repo base directory
$ conda env update
```

### Deploy

To deploy the site we use the command `nikola github_deploy -m "CHANGES"` (from inside the repo directory with the environment activated).
