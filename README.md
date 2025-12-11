# Website of the IEEE Student Branch Karlsruhe

This repository contains the sources of our website. It is build using the static site generator [Nikola](https://getnikola.com/). And deployed to the branch gh-pages and available on http://ieee-ka.de

### Build

1. Create python virutal environment and install with requirements:
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
use Ctrl + c to end browser

### Deploy

To deploy the site we use the command `nikola github_deploy -m "CHANGES"` (from inside the repo directory with the environment activated).
