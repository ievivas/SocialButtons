# Social Buttons
Nice and simple CSS3 social buttons with transitions and transforms.

Click the image bellow to see to see the buttons in action:

[![Buttons in action](http://ivanvivas.site90.com/socialButtons.png)](http://ivanvivas.site90.com/socialButtons.html)

Author [Ivan Vivas](https://twitter.com/ievivas)

## Include buttons in your website
Copy and paste the code in your website files:

### HTML
```
<div id="social-buttons">
	<div class="circle facebook">
		<a href="" target="_blank" title="Facebook">
			<span class="ion-social-facebook"></span>
		</a>
	</div>
	<div class="circle twitter">
		<a href="" target="_blank" title="Twitter">
			<span class="ion-social-twitter"></span>
		</a>
	</div>
	<div class="circle instagram">
		<a href="" target="_blank" title="Instagram">
			<span class="ion-social-instagram"></span>
		</a>
	</div>
	<div class="circle google-plus">
		<a href="" target="_blank" title="Google +">
			<span class="ion-social-googleplus"></span>
		</a>
	</div>
	<div class="circle github">
		<a href="" target="_blank" title="Github">
			<span class="ion-social-github"></span>
		</a>
	</div>
	<div class="circle whatsapp">
		<a href="" target="_blank" title="Whatsapp">
			<span class="ion-social-whatsapp"></span>
		</a>
	</div>
</div>
```

### SCSS
```
$color-facebook: rgb(59,89,152);
$color-twitter: rgb(64,153,255);
$color-instagram: rgb(155, 105, 84);
$color-google-plus: rgb(211, 72, 54);
$color-github: black;
$color-whatsapp: rgb(77, 194, 71);

@mixin limpiar() {
	margin: 0px;
	padding: 0px;
}

@mixin dimensiones($ancho, $alto) {
	width: $ancho;
	height: $alto;
}

@mixin circulo($color, $diametro) {
	-webkit-border-radius: 50%;
	-moz-border-radius: 50%;
	-ms-border-radius: 50%;
	border-radius: 50%;
	background-color: $color;
	height: $diametro;
	width: $diametro;
}

#social-buttons {
	background-color: grey;
	text-align: center;
	.circle {
		@include limpiar();
		@include circulo(none, 50px);
		border: 2px solid white;
		text-align: center;
		display: inline-block;
		margin: 5px;
		a {
			text-decoration: none;
			color: white;
			span {
				font-size: 25px;
				//Las sig. 2 lineas son para aumentar el area cliqueable
				display: block;
				@include dimensiones(100%, 100%);
				padding-top: 10px;
			}
		}
	}
	.facebook {
		-webkit-transition: transform 0.5s, background-color 0.5s;
		-moz-transition: transform 0.5s, background-color 0.5s;
		-ms-transition: transform 0.5s, background-color 0.5s;
		transition: transform 0.5s, background-color 0.5s;
		&:hover {
			background-color: $color-facebook;
			-webkit-transform: scale(1.3,1.3) rotate(360deg);
			-moz-transform: scale(1.3,1.3) rotate(360deg);
			-ms-transform: scale(1.3,1.3) rotate(360deg);
			transform: scale(1.3,1.3) rotate(360deg);
		}
	}
	.twitter {
		-webkit-transition: transform 0.5s, background-color 0.5s;
		-moz-transition: transform 0.5s, background-color 0.5s;
		-ms-transition: transform 0.5s, background-color 0.5s;
		transition: transform 0.5s, background-color 0.5s;
		&:hover {
			background-color: $color-twitter;
			-webkit-transform: scale(1.3,1.3) rotate(360deg);
			-moz-transform: scale(1.3,1.3) rotate(360deg);
			-ms-transform: scale(1.3,1.3) rotate(360deg);
			transform: scale(1.3,1.3) rotate(360deg);
		}
	}
	.instagram {
		-webkit-transition: transform 0.5s, background-color 0.5s;
		-moz-transition: transform 0.5s, background-color 0.5s;
		-ms-transition: transform 0.5s, background-color 0.5s;
		transition: transform 0.5s, background-color 0.5s;
		&:hover {
			background-color: $color-instagram;
			-webkit-transform: scale(1.3,1.3) rotate(360deg);
			-moz-transform: scale(1.3,1.3) rotate(360deg);
			-ms-transform: scale(1.3,1.3) rotate(360deg);
			transform: scale(1.3,1.3) rotate(360deg);
		}
	}
	.google-plus {
		-webkit-transition: transform 0.5s, background-color 0.5s;
		-moz-transition: transform 0.5s, background-color 0.5s;
		-ms-transition: transform 0.5s, background-color 0.5s;
		transition: transform 0.5s, background-color 0.5s;
		&:hover {
			background-color: $color-google-plus;
			-webkit-transform: scale(1.3,1.3) rotate(360deg);
			-moz-transform: scale(1.3,1.3) rotate(360deg);
			-ms-transform: scale(1.3,1.3) rotate(360deg);
			transform: scale(1.3,1.3) rotate(360deg);
		}
	}
	.github {
		-webkit-transition: transform 0.5s, background-color 0.5s;
		-moz-transition: transform 0.5s, background-color 0.5s;
		-ms-transition: transform 0.5s, background-color 0.5s;
		transition: transform 0.5s, background-color 0.5s;
		&:hover {
			background-color: $color-github;
			-webkit-transform: scale(1.3,1.3) rotate(360deg);
			-moz-transform: scale(1.3,1.3) rotate(360deg);
			-ms-transform: scale(1.3,1.3) rotate(360deg);
			transform: scale(1.3,1.3) rotate(360deg);
		}
	}
	.whatsapp {
		-webkit-transition: transform 0.5s, background-color 0.5s;
		-moz-transition: transform 0.5s, background-color 0.5s;
		-ms-transition: transform 0.5s, background-color 0.5s;
		transition: transform 0.5s, background-color 0.5s;
		&:hover {
			background-color: $color-whatsapp;
			-webkit-transform: scale(1.3,1.3) rotate(360deg);
			-moz-transform: scale(1.3,1.3) rotate(360deg);
			-ms-transform: scale(1.3,1.3) rotate(360deg);
			transform: scale(1.3,1.3) rotate(360deg);
		}
	}
}
```

### CSS
```
#social-buttons {
  background-color: grey;
  text-align: center;
}

#social-buttons .circle {
  margin: 0px;
  padding: 0px;
  -webkit-border-radius: 50%;
  -moz-border-radius: 50%;
  -ms-border-radius: 50%;
  border-radius: 50%;
  background-color: none;
  height: 50px;
  width: 50px;
  border: 2px solid white;
  text-align: center;
  display: inline-block;
  margin: 5px;
}

#social-buttons .circle a {
  text-decoration: none;
  color: white;
}

#social-buttons .circle a span {
  font-size: 25px;
  display: block;
  width: 100%;
  height: 100%;
  padding-top: 10px;
}

#social-buttons .facebook {
  -webkit-transition: transform 0.5s, background-color 0.5s;
  -moz-transition: transform 0.5s, background-color 0.5s;
  -ms-transition: transform 0.5s, background-color 0.5s;
  transition: transform 0.5s, background-color 0.5s;
}

#social-buttons .facebook:hover {
  background-color: #3b5998;
  -webkit-transform: scale(1.3, 1.3) rotate(360deg);
  -moz-transform: scale(1.3, 1.3) rotate(360deg);
  -ms-transform: scale(1.3, 1.3) rotate(360deg);
  transform: scale(1.3, 1.3) rotate(360deg);
}

#social-buttons .twitter {
  -webkit-transition: transform 0.5s, background-color 0.5s;
  -moz-transition: transform 0.5s, background-color 0.5s;
  -ms-transition: transform 0.5s, background-color 0.5s;
  transition: transform 0.5s, background-color 0.5s;
}

#social-buttons .twitter:hover {
  background-color: #4099ff;
  -webkit-transform: scale(1.3, 1.3) rotate(360deg);
  -moz-transform: scale(1.3, 1.3) rotate(360deg);
  -ms-transform: scale(1.3, 1.3) rotate(360deg);
  transform: scale(1.3, 1.3) rotate(360deg);
}

#social-buttons .instagram {
  -webkit-transition: transform 0.5s, background-color 0.5s;
  -moz-transition: transform 0.5s, background-color 0.5s;
  -ms-transition: transform 0.5s, background-color 0.5s;
  transition: transform 0.5s, background-color 0.5s;
}

#social-buttons .instagram:hover {
  background-color: #9b6954;
  -webkit-transform: scale(1.3, 1.3) rotate(360deg);
  -moz-transform: scale(1.3, 1.3) rotate(360deg);
  -ms-transform: scale(1.3, 1.3) rotate(360deg);
  transform: scale(1.3, 1.3) rotate(360deg);
}

#social-buttons .google-plus {
  -webkit-transition: transform 0.5s, background-color 0.5s;
  -moz-transition: transform 0.5s, background-color 0.5s;
  -ms-transition: transform 0.5s, background-color 0.5s;
  transition: transform 0.5s, background-color 0.5s;
}

#social-buttons .google-plus:hover {
  background-color: #d34836;
  -webkit-transform: scale(1.3, 1.3) rotate(360deg);
  -moz-transform: scale(1.3, 1.3) rotate(360deg);
  -ms-transform: scale(1.3, 1.3) rotate(360deg);
  transform: scale(1.3, 1.3) rotate(360deg);
}

#social-buttons .github {
  -webkit-transition: transform 0.5s, background-color 0.5s;
  -moz-transition: transform 0.5s, background-color 0.5s;
  -ms-transition: transform 0.5s, background-color 0.5s;
  transition: transform 0.5s, background-color 0.5s;
}

#social-buttons .github:hover {
  background-color: black;
  -webkit-transform: scale(1.3, 1.3) rotate(360deg);
  -moz-transform: scale(1.3, 1.3) rotate(360deg);
  -ms-transform: scale(1.3, 1.3) rotate(360deg);
  transform: scale(1.3, 1.3) rotate(360deg);
}

#social-buttons .whatsapp {
  -webkit-transition: transform 0.5s, background-color 0.5s;
  -moz-transition: transform 0.5s, background-color 0.5s;
  -ms-transition: transform 0.5s, background-color 0.5s;
  transition: transform 0.5s, background-color 0.5s;
}

#social-buttons .whatsapp:hover {
  background-color: #4dc247;
  -webkit-transform: scale(1.3, 1.3) rotate(360deg);
  -moz-transform: scale(1.3, 1.3) rotate(360deg);
  -ms-transform: scale(1.3, 1.3) rotate(360deg);
  transform: scale(1.3, 1.3) rotate(360deg);
}
```
