# Semantic

A Python library for extracting semantic information from text, such as dates and numbers. Full documentation is available on [PIP](https://pythonhosted.org/semantic/), with a list of primary features below.

[![Build Status](https://travis-ci.org/crm416/semantic.png)](https://travis-ci.org/crm416/semantic.png)

[![PyPI version](https://badge.fury.io/py/semantic.png)](http://badge.fury.io/py/semantic)

# Installation

Installing semantic is simple

    $ pip install semantic

# Features

semantic consists of four main modules, each of which corresponds to a different semantic extractor.

## Dates (_date.py_)
- Extracting relative (e.g., "a week from today") and absolute (e.g., "December 11, 2013") dates from text snippets.
- Converting date objects to human-ready phrasing.

## Numbers (_number.py_)
- Extracting numbers (integers or floats) from text snippets.
	- E.g.: From "Two hundred and six" to 206.
	- E.g.: From "Five point one five" to 5.15.
	- E.g.: From "Eleven and two thirds" to 11.666666666666666.
- Converting numbers to human-readable strings.
	- E.g.: From "7e-05" to "seven to the negative five".

## Math (_solver.py_)
- Performing mathematical operations expressed as words.
	- E.g.: From "Log one hundred and ten" to Log(110) = 4.70048.

## Units (_units.py_)
- Converting between units expressed as words.
	- E.g.: From "Seven and a half kilograms to pounds" to 16.5347.
    - E.g.: From "Seven and a half pounds per square foot to kilograms per meter squared" to 36.618.

# Usage

The test suite (_test.py_) contains tons of examples and use-cases for each of the four modules.

The Dates, Numbers, and Math modules can run in isolation (i.e., without any dependencies), while the Units module requires [quantities](https://pypi.python.org/pypi/quantities) and [Numpy](http://www.numpy.org).

# License

MIT © [Charles Marsh](https://github.com/crm416)