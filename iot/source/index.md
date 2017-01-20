---
title: Programming the Cloud : WEB

language_tabs:
  - shell: Terminal
  - css: CSS 
  - html: HTML
  - javascript: Javascript
  - json: JSON

toc_footers:

includes:
  - _kit

search: true
---




# Introduction 

This guide will introduce you to front-end and back-end web
technologies. Figure 1 show the different technologies we will be using.

# Motivation

# The Modern Web

## History of the Web (10)

## The client-server model (10)

## The Browser (10)

## Web Server (20)


# HTML and CSS — Designing for the web

## HTML5

The Hypertext Transfer Protocol outlines the framework for web-servers, browsers, apps and  to transfer web-pages and 


## Concurrent Style Sheets

### Embed in HTML

### jsFiddle

### CSS Animations

### jQuery

### Responsive Design

#### CSS Media queries

#### jQuery


# Javascript — Coding for the web

## Programming basics

### Doing Arithmetic

### Operators

### Execution sequence

### Simple Statements

### Variables, literals, constants

### Complex Statements

### Functions and Closures

### Objects

### User input

### Putting it all together 

### Callbacks

### Event model
              



##   Integrating third-party libraries (GIT)

##   Customization via device detection



# Server-side JavaScript (Node.js)

## Basic HTTP server

## NPM

## Express.js

## Data persistence (mongoDB)

## Using Amazon Web Services

### EC2

### S3

### SNS

### SES

# Data Structures & Algorithms

## Lists

## Queue

## Stacks

## Trees

## Graphs

## Sorting

### bubble sort

### insertion sort

### selection sort

## Sorting and Filtering Lists




# Advanced Topics

## Less 

## Bootstrap

## Anappfor.me

## Native-esque apps using web technologies (Apache Cordova)

## Building JS Libraries


> To authorize, use this code:

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

Kittn uses API keys to allow access to the API. You can register a new Kittn API key at our [developer portal](http://example.com/developers).

Kittn expects for the API key to be included in all API requests to the server in a header that looks like the following:

`Authorization: meowmeowmeow`

<aside class="notice">
You must replace <code>meowmeowmeow</code> with your personal API key.
</aside>

# Kittens

## Get All Kittens

```css
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
api.kittens.get
```

```html
import kittn

api = kittn.authorize('meowmeowmeow')
api.kittens.get()
```

```shell
curl "http://example.com/api/kittens"
  -H "Authorization: meowmeowmeow"
```

> The above command returns JSON structured like this:

```js
[
  {
    "id": 1,
    "name": "Fluffums",
    "breed": "calico",
    "fluffiness": 6,
    "cuteness": 7
  },
  {
    "id": 2,
    "name": "Isis",
    "breed": "unknown",
    "fluffiness": 5,
    "cuteness": 10
  }
]
```

This endpoint retrieves all kittens.

### HTTP Request

`GET http://example.com/api/kittens`

### Query Parameters

| Parameter | Default | Description |
| ---- | ---- | ---- |
| include_cats | false | If set to true, the result will also include cats. |
| available | true | If set to false, the result will include kittens that have already been adopted. |

<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

## Get a Specific Kitten

```css
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
api.kittens.get(2)
```

```html
import kittn

api = kittn.authorize('meowmeowmeow')
api.kittens.get(2)
```

```shell
curl "http://example.com/api/kittens/2"
  -H "Authorization: meowmeowmeow"
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "name": "Isis",
  "breed": "unknown",
  "fluffiness": 5,
  "cuteness": 10
}
```

This endpoint retrieves a specific kitten.

<aside class="warning">If you're not using an administrator API key, note that some kittens will return 403 Forbidden if they are hidden for admins only.</aside>

### HTTP Request

`GET http://example.com/kittens/<ID>`

### URL Parameters

Parameter | Description
---- | ----
ID | The ID of the kitten to retrieve

