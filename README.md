# cab.cab

## Plone Website

* `Source code @ GitHub <https://github.com/kreativkombinat/cab.cab>`_
* `Releases @ PyPI <http://pypi.python.org/pypi/cab.cab>`_
* `Documentation @ ReadTheDocs <http://cabcab.readthedocs.org>`_
* `Continuous Integration @ Travis-CI <http://travis-ci.org/kreativkombinat/cab.cab>`_

## How it works

This project templates provides a full blown Plone project environment. I tcomes with a preconfigured project specific theme package located under the _src_ directory. 

In order to get started you need to first generate a project environment:

```bash
$ cd src/
$ $ mrbob --config ~/.mrbob builodut.projectname bobtemplate:plone
```

Answer the questions *mr.bob* might have for you concerning the desired target production host and port settings.

After *mr.bob* is done you can import the generated plone project into your SCM.


## Installation

This buildout is intended to be used via the development profile to provide
a ready to work on setup. The relevant steps to get started with a new
development environment would be:

``` bash
$ virtualenv-2.7 cab
$ cd ./cab
$ git clone gitlgithub.com:username/cab.cab.git cab.cab
$ cd ./cab.cab
$ python bootstrap.py -c development.cfg
$ bin/buildout -Nc development.cfg
```


## Configuration

The generated buildout asumes that the developer has setup a local egg cache and therefore provides a buildout 'default.cfg'.
