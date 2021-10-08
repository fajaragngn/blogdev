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
  <style>

    body.darkmode {
        background: rgb(57, 57, 57);
        color: rgb(227, 227, 227);
    }

    a{
        color: rgb(87, 87, 87);
    }

    body.darkmode a{
        color: rgb(227, 227, 227);
    }

    .is-hidden{
        display: none;
    }



    #theme {
        font-size: 20px;
    }

    #theme:hover {
        cursor: pointer
    }
  </style>
</head> 
<body>
  
<header>
  <script>
  	if(localStorage.getItem('preferredTheme') == 'dark') {
    	setDarkMode(true)
    }

    function setDarkMode(isDark) {
        var darkBtn = document.getElementById('darkBtn')
        var lightBtn = document.getElementById('lightBtn')

        if(isDark) {
            lightBtn.style.display = "block"
            darkBtn.style.display = "none"
            localStorage.setItem('preferredTheme', 'dark');
        } else {
            lightBtn.style.display = "none"
            darkBtn.style.display = "block"
            localStorage.removeItem('preferredTheme');
        }

        document.body.classList.toggle("darkmode");
    }
</script>
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

 
</body> 
</html>