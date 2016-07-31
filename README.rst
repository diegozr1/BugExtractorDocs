Bug Extractor
========
https://github.com/TaskAssignment/BugExtractor


The bug extractor is a Python3 script used to extract the information


Installation
----

To install and run the bug extractor:


Clone the repository::

    $ git clone https://github.com/TaskAssignment/BugExtractor

Change the directory::

    $ cd BugExtractor

Install the packages with pip::

    $ pip3 install -r requirements.txt


Use
--------

Show services available::

    $ python3 generalextractor.py showservices

Show projects from a service::

    $ python3 generalextractor.py showprojects mozilla

Extract complete list of bugs from a service (Might take several hours)::

    $ python3 generalextractor.py mozilla

Extract bugs from a specific project inside a service (Might take up to 1 hour)::

    $ python3 generalextractor.py mozilla firefox


**When any of this commands are runned the information is saved to
spreadsheets (TSV file) and save to the main TaskAssignment mongo
database with the schema indicated**


*This example uses mozilla this can be changed to eclipse or any other when supported*


Services available
--------

- mozilla
- eclipse

The rest of projects hosted on Bugzilla might work
but are not tested and completely supported


Projects
----------

These are example projects in Mozilla

- Firefox
- Thunderbird
- Toolkit

Examples
-------

- python3 generalextractor.py mozilla
- python3 generalextractor.py mozilla thunderbird
- python3 generalextractor.py mozilla tookit


Troubleshooting
-------

If this script runs in any problem let me know
