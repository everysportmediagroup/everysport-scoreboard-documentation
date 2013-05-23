# Today's Games

The following Web page displays today's games only, in a 320px wide area: 

```html
<!DOCTYPE html>
<html>
<head>  
    <meta name="viewport" content="initial-scale=1.0" /> 
  <style style="text/css">
    body {
    font-size: 100%;
    font-family: sans-serif;
    }

    div.everysport-calendar {
      width: 320px;
      margin: 0 auto;
    }
  </style>
</head>
<body>

<div class="everysport-calendar"></div>

<script>
var esApiKey = "{DIN APIKEY}";
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