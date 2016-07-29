Bug Extractor
========
https://github.com/TaskAssignment/BugExtractor


The bug extractor is a Python3 script used to extract the information


Installation
----

To install and run the bug extractor:


Clone the repository::

    $ git clone https://github.com/TaskAssignment/BugExtractor

Change the directory

    $ cd BugExtractor

Install the packages with pip::

    $ pip3 install -r requirements.txt


Use
--------

Show services available::

  $  python3 generalextractor.py [service] [projects]

Show services from every project::

  $ cd IssuesProvider


Extract bugs from a service ::

    $ python3 generalextractor.py [service]

Run the program with::

    $ npm start

The api will be available at

  "http://localhost:3000"


To make use of the API just follow these rules


Services available
--------

- Mozilla
- Eclipse

The rest of projects hosted on Bugzilla might work
but are not tested and completely supported


Contribute
----------

- Issue Tracker: github.com/$project/$project/issues
- Source Code: github.com/$project/$project

Support
-------

If you are having issues, please let us know.
We have a mailing list located at: project@google-groups.com

License
-------

The project is licensed under the BSD license.
