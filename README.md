# Balena Server Pi2

This repository contains all the tools to build a Balena container project designed to run on a Raspberry Pi Zero W.

This project is designed to build a Server device, running the Pi2.py file on a Raspberry Pi, which creates and runs a Python Flask web-app. This device acts as a Server and Sink in a Server-client architecure, connecting to a second 'Client' device, which samples temperature and light level data (also inside a Balena container). The sensor samples collected by this device are sent to this server using Python TCP sockets.

The project contains a dockerfile template, which creates a Dockerfile used to install the libraries necessary for creating a Flask webserver, and to run the python script Pi2.py.

This project should print out the url of the Flask webserver, which can also be accessed on the Balena webportal.

The server-client interaction can be monitored from the Balena webportal.

**Authors**: James Burness, Jacq van Jaarsveld

**Project**: EEE3095S Practical 6
