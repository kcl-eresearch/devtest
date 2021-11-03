Developer test
===

Welcome to the King's e-research developer test.
We have a Flask application here (under the "devtest" folder) and a few support tickets (under the "tickets" folder).
Have a look in the "tickets" folder, there you will find your tasks to complete.
Once you have completed the tickets, please either zip this folder and send it to me (Skylar) or send a diff.

How to run the application
====
In order to complete these tasks you will need to run Flask.
There are two ways to do this, either DIY or use the included Dockerfile.
Once you run the application, you can go to http://127.0.0.1:5000/ in your browser to view the portal.
These steps have only been tested on Ubuntu. It is expected that you will have a Linux device of some kind, whether it be a full PC or a VM. If not we recommend provisioning a Virtualbox VM for the purposes of this test.

Docker
====
 - docker build -t devtesti .
 - docker run -d --name devtest -p 5000:80 devtesti

DIY (Linux)
=====
 - Install poetry: `curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/install-poetry.py | python -`
 - Run `poetry install` in this directory
 - To run the application: `FLASK_APP=devtest poetry run flask run`
