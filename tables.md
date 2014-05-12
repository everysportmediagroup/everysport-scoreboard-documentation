# Table

If you just want to show the table for a specific league, hide the menu and the events, and launch the scoreboard with the League ID. 

The following code example displays the Allsvenskan (63925) table.


```html
<div class="everysport-scoreboard" data-league-selected="63925" data-hide-menu="true"  data-hide-events="true" data-hash-tag="false"></div>

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
```

Change ```data-hide-events``` to false to show upcoming games below the table.