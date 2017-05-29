---
title: Programming the Cloud : IoT

language_tabs:
  - shell: Terminal
  - css: CSS 
  - html: HTML
  - javascript: Node.js
  - json: JSON

toc_footers:

includes:
  - _kit
  - _class

search: true
---




# Introduction 

This guide will introduce you to front-end and back-end web
technologies. Figure 1 show the different technologies we will be using.

# Motivation


# Tools/Technologies 

## Arduino IDE

## esptool.py

## AWS EC2

## AWS Lambda

## Node.js

## mongoDB

> To authorize, use this code:

# IoT Experiments

## Hello World
### Hello World - Server
  A simple HTTP server that send the string "Hello World" as response to
every http GET request.

<aside class="notice">
 <i> Client server model </i>


<img
src="https://upload.wikimedia.org/wikipedia/commons/c/c9/Client-server-model.svg"
align="center" height="248" width="auto" >

The Client server model is the backbone of the World Wide Web (www) and
is one of the most important protocols to comminucate withg
Internet-enabled 'Things'. The server is a program (not necessarily
running on a 'big' computer, but any Microprocessor/Microcontroller)
that can receive requests at a specific port, and respond back to the
client that sent the request. The most common example of this is HTTP
servers that send file data (HTML, images, js, css etc.) like
google.com, yahoo.com or any other web server. This guide will teach you
how to write 'Web Services' that can interact with your
Internet-connected Things.
</aside>


Starting by installing Node.js ([install instructions](#node-js)) on
your machine. We will write a server that listens to
localhost(127.0.0.1) at post 8080 (see aside on URLs).

<aside class="notice">
Uniform Resource Locator (URL)
</aside>
### Hello World - Internet connected MCU

## Scan for Wifi Networks

## Turn on/off LED via Web-server

## Turn on/off LED via Internet

## Internet connected Push Button

## Push button to send email

## Push Button to send temperature/humidity as email

## Graphing temperature and humidity

## Logging sensor values in a database

## Sending alerts when certain values are out of range

## Dimming LEDs with Pulse Width Modulation (PWM)

## Control RGB lights

## Play MIDI over the Internet

## Turn on/off any AC device using relay

## Control 2 color LED

## Control 1-bit display

## Use 7 color flash to alert high temperature (IR LED)

## Use Tap module to send morse-code to server

## Automatic light switch (with data logging)

## Motion switch (with data logging)

## Shock sensors for logging shocks

## Internet enabled touch switch (with hot keys)

## A blind navigation tool (with data logging)

## Control fan speed with a magnet (with data logging)

## Connected home --  control LEDs with Echo

## More to come
  The componets in the IoT starter kit can be used for many more
experiments. If you want your experiment to be featured here, please
submit your experiment [here]().

```shell
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
```

```js
import kittn

api = kittn.authorize('meowmeowmeow')
```

```shell
# With shell, you can just pass the correct header with each request
curl "api_endpoint_here"
  -H "Authorization: meowmeowmeow"
```

> Make sure to replace `meowmeowmeow` with your API key.

