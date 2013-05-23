# Getting Started
The following Web page displays the Scoreboard. It lets the user choose a sport and then a league, to see the latest standings and upcoming games:

```html
<!DOCTYPE html>
<html>
<head>  
   <meta name="viewport" content="initial-scale=1.0" /> 
  <style style="text/css">
    	body {
    		font-size: 90%;
    		font-family: sans-serif;
        max-width: 640px;
  		}
  </style>
</head>
<body>

<div class="everysport-scoreboard"></div>

<script>
var esApiKey = "{YOUR APIKEY}";
(function(d, t) {
  	  var g = d.createElement(t),
    	    s = d.getElementsByTagName(t)[0];
    	g.src = 'http://v1.tpl.everysport.com/js/scoreboard-all.js';
    	g.charset = 'utf-8';
    	s.parentNode.insertBefore(g, s);
}(document, 'script'));
</script>
</body>
</html>
```

Note the following: 
* The Scoreboard is included using a <script> tag.
* A <div> element with CSS class 'everysport-scoreboard' holds the Scoreboard. 
* The width and font size is set by CSS on the Scoreboard <div> element.   








