+++
Description = ""
categories = ["docs"]
date = 2020-11-03T17:00:00Z
featured_image = ""
tags = ["darkmode", "website"]
title = "Dark mode pada website"

+++
| --- |
| <!DOCTYPE html> |
|  | <html> |
|  | <meta charset="UTF-8"> |
|  | <meta name="viewport" content="width=device-width, initial-scale=1.0"> |
|  | <head> |
|  | <title>Simple dark mode</title> |
|  | </head> |
|  | <link rel="stylesheet" type="text/css" href="assets/css/main.css"> |
|  | <body> |
|  |  |
|  | <header> |
|  | <div> |
|  | <a href="/">/@fajar.agngn</a> |
|  | </div> |
|  | <div id=theme> |
|  | <div onclick=setDarkMode(true) id=darkBtn> |
|  | <a>dark/</a> |
|  | </div> |
|  | <div onclick=setDarkMode(false) id=lightBtn class=is-hidden> |
|  | <a>/light</a> |
|  | </div> |
|  | </div> |
|  | </header> |
|  |  |
|  | <h1>Hi there.</h1> |
|  |  |
|  | <script type="text/javascript" src="assets/js/main.js"></script> |
|  | </body> |
|  | </html> |
