# Getting Started
The following Web page displays the Scoreboard. It lets the user choose a sport and then a league, to see the latest standings and upcoming games:

```html
<!DOCTYPE html>
<html>
<head>  

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
* The Scoreboard is included using a `<script>` tag.
* A `<div>` element with CSS class 'everysport-scoreboard' holds the Scoreboard. 
* The width and font size is set by CSS on the Scoreboard `<div>` element.   



## Pre-selected league

Use the ```data-league-selected```attribute to start the scoreboard with a pre-selected league. In this example 60243 is the Everysport league ID for SHL, the Swedish Hockey League.  

```html
<div class="everysport-scoreboard" data-league-selected="60243"></div>
```

## Pre-selected sport

Use the ```data-sport-selected```attribute to start the scoreboard with a pre-selected sport. In this example 2 is Hockey.  

```html
<div class="everysport-scoreboard" data-sport-selected="2"></div>
```
The sport IDs are defined [here]("https://github.com/menmo/everysport-api-documentation/blob/master/endpoints/GET_sports.md")



## Pre-selected team

Use the ```data-team``` attribute to launch the scoreboard with the current standings and events for a specific team. The attribute should contain the Everysport team Id.


```html
<div class="everysport-scoreboard" data-team="9375"></div>
```



## Hide menu / topbar

Use the ```data-hide-menu``` attribute to hide the menu. This is ideal for including the scoreboard in articles related to a specific league.

```html
<div class="everysport-scoreboard" data-league-selected="60243" data-hide-menu="true"></div>
```

## Hide events or standings 

User ```data-hide-events``` or ```data-hide-standings``` to hide the respective section. For example, to show only the table, hide the events. 

```html
<div class="everysport-scoreboard" data-league-selected="60243" data-hide-menu="true" data-hide-events="true"></div>
```

## Disable URL hash 

User ```data-hash-tag``` to disable that the scoreboard updated the URL when the user navigates. 

```html
<div class="everysport-scoreboard" data-league-selected="60243" data-hash-tag="false"></div>
```











