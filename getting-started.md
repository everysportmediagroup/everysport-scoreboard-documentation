# Getting Started
The following code embeds the Scoreboard:
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



