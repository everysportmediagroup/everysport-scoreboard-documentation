# Presentation
You can change the presentation of the Scoreboard in two ways:

1. With CSS on the scoreboard element. By default the Scoreboard inherits style from the CSS of its parent elements 
2. With presentational ```data-```-attributes on the scoreboard element. 

## Changing fonts and size with standard CSS
The following presentational properties of the Scoreboard can be changed with standard CSS:
* Font family (i.e. typeface)
* Font size 
* Width
* Margin and paddings

The following CSS code sets the font-size to exactly 12px, the font family to Serif and the width to 280px: 

```html
	div.everysport-scoreboard {
		width: 280px;
		font-size: 12px; 
		margin: 1em auto;
		font-family: serif; 
	}
```

## Changing Top-bar colors with data-attributes  
You can change the background- and text-color of the top-bar of the Scoreboard by using the ```data-color``` and ```data-background-color``` attributes on the scoreboard element. 

```html
<div class="everysport-scoreboard" data-color="black" data-background-color="white" ></div>
```

   




