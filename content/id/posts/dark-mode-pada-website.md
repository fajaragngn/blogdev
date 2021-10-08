+++
Description = ""
categories = ["docs"]
date = 2020-11-03T17:00:00Z
featured_image = ""
tags = ["darkmode", "website"]
title = "Dark mode pada website"

+++

<html>
<meta charset="UTF-8"> 
<meta name="viewport" content="width=device-width, initial-scale=1.0"> 
<head> 
</head>
<link rel="stylesheet" type="text/css" href="assets/css/main.css"> 
<body>
  <style>
    body{
      margin: 3% auto;
      width: 60%;
      font-size: 1.2rem;
      line-height: 1.8rem;
      font-family: arial;
      color: rgb(87, 87, 87);
      background: #faf9f5;
    }

    body.darkmode {
        background: rgb(57, 57, 57);
        color: rgb(227, 227, 227);
    }

    a{
        color: rgb(87, 87, 87);
    }
    h1{
        text-align: center;
        margin: 30% auto;
    }
    body.darkmode a{
        color: rgb(227, 227, 227);
    }

    .is-hidden{
        display: none;
    }

    header{
        display: flex;
        justify-content: space-between;
        margin-bottom: 20px;
        font-size: 20px;
    }

    #theme {
        font-size: 20px;
    }

    #theme:hover {
        cursor: pointer
    }
  </style>
<header>
<div>
<a href="/">/@fajar.agngn</a>
</div>
<div id=theme> 
<div onclick=setDarkMode(true) id=darkBtn> 
<a>dark/</a> 
</div> 
<div onclick=setDarkMode(false) id=lightBtn class=is-hidden> 
<a>/light</a> 
</div> 
</div>
</header> 

<h1>Hi there.</h1> 

<script type="text/javascript" src="assets/js/main.js"></script> 
</body> 
</html> 