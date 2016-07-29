============
IssuesProvider
============
https://github.com/TaskAssignment/IssuesProvider


The issuesprovider is an API that integrates all the bugs found in the repositories hosted
in Github, BugZilla and Gitlab

Clone the repository::

  $  git clone https://github.com/TaskAssignment/IssuesProvider

Change directory into it::

  $ cd IssuesProvider


Install the packages with npm::

    $ npm install

Run the program with::

    $ npm start

The api will be available at

  "http://localhost:3000"


To make use of the API just follow these rules

List of routes
--------------

The api is under "/api/v1"
Services

    - /api/v1/service/:service/:user/repos
    - /api/v1/service/:service/:user/:repo/bugs
    - /api/v1/service/:service/:user/:repo/users

List of services
----------------

    - github
    - bitbucket
    - gitlab

Products
--------

    - /api/v1/product/:product/:component/bugs
    - /api/v1/product/:product/:project/bugs

List of products
----------------

    - bugparty
    - bugzilla
    - eclipse


Examples
--------

    - /api/v1/github/robfz/repos
    - /api/v1/gitlab/2rbdPSvGXzbxYSCUoszC/repos
    - /api/v1/bitbucket/abram

    - /api/v1/gitlab/2rbdPSvGXzbxYSCUoszC/1206370/bugs
    - /api/v1/github/rails/rails/bugs
    - /api/v1/bitbucket/zdr00/menubarmac/bugs


Important
---------

- For the gitlab service you don't have to provide your username but your access_token you can grab it at

"https://gitlab.com/profile/account" or "/api/v1/gitlab/token/:user/password/"

- There is also a url to login at gitlab "/gitlab/token/:user/password/" to get the private_token of a user

"*bugparty" needs to be deployed to the cloud before using it

- for "bugparty" endpoints provide "#" instead of the user and the project instead of repoid

"bugparty" provides a bit different information about the repos

- "*bugzilla" bugs need to be specified by product for example "bugzilla" or "thunderbird"
