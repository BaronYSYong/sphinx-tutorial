# Sphinx

## Reference
* https://pythonhosted.org/an_example_pypi_project/sphinx.html
* http://www.sphinx-doc.org/en/stable/tutorial.html
* http://www.sphinx-doc.org/en/stable/ext/math.html
* https://thomas-cokelaer.info/tutorials/sphinx/docstring_python.html
* http://blog.amedama.jp/entry/2015/10/15/212527

## Installation
```
$ pip install Sphinx
```

## Quick Start
```
$ sphinx-quickstart
```
Please enter values for the following settings (just press Enter to
accept a default value, if one is given in brackets).
```
> Root path for the documentation [.]: ENTER
> Separate source and build directories (y/n) [n]: y
> Name prefix for templates and static dir [_]: ENTER
> Project name: Example
> Author name(s): Baron Yong
> Project version []: 0.0.1
> Project release [0.0.1]: ENTER
> Project language [en]: ENTER
> Source file suffix [.rst]: ENTER
> Name of your master document (without suffix) [index]: ENTER
> Do you want to use the epub builder (y/n) [n]: ENTER

Please indicate if you want to use one of the following Sphinx extensions:
> autodoc: automatically insert docstrings from modules (y/n) [n]: y
> doctest: automatically test code snippets in doctest blocks (y/n) [n]: ENTER
> intersphinx: link between Sphinx documentation of different projects (y/n) [n]: ENTER
> todo: write "todo" entries that can be shown or hidden on build (y/n) [n]: ENTER
> coverage: checks for documentation coverage (y/n) [n]: ENTER
> imgmath: include math, rendered as PNG or SVG images (y/n) [n]: ENTER
> mathjax: include math, rendered in the browser by MathJax (y/n) [n]: ENTER
> ifconfig: conditional inclusion of content based on config values (y/n) [n]: y
> viewcode: include links to the source code of documented Python objects (y/n) [n]: ENTER
> githubpages: create .nojekyll file to publish the document on GitHub pages (y/n) [n]: ENTER

A Makefile and a Windows command file can be generated for you so that you
only have to run e.g. `make html' instead of invoking sphinx-build
directly.
> Create Makefile? (y/n) [y]: y
> Create Windows command file? (y/n) [y]: n
```
Uncomment below in conf.py
```
import os
import sys
sys.path.insert(0, os.path.abspath('.'))
```
Create a file called code.rst and paste below into it
```
Documentation for the Code
**************************
.. automodule:: Algorithm.template
   :members:

```
