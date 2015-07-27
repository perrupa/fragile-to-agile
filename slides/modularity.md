<!-- .slide: data-background-image="/images/BG/pipes.jpg" -->
# Modularity

---

## Much of the power of the UNIX operating system comes from a style of program design that makes programs easy to use and, more important, easy to combine with other programs.

#### Program Design in the UNIX Environment

---

## Reusability
<br>
## Consistency
<br>
## Speed of Development

---

<!-- .slide: data-background-image="/images/BG/breakin2.jpg" -->
# Pattern Library 2
### Electric Boogaloo

---

<!-- .slide: data-background-image="/images/BG/turtle-sandbox.jpg" -->
## Sandboxing

---

<!-- .slide: data-background-image="/images/BG/dev-sandbox.jpg" -->
## Inside the platform
<br>
## Free of external influences
<br>
## Guaranteed portability of Code

---

<!-- .slide: data-background-image="/images/BG/lego.jpg" -->
# OOCSS 

---

<!-- .slide: data-background-image="/images/BG/framework.jpg" -->
## OOCSS concept:
<br>
#Decouple the CSS from the HTML

---


```sass
.userSelect-dropdown li {
	//Style list items in the dropdown
}
```

---

<!-- .slide: data-background-image="/images/BG/dad-dog.jpg" -->
## And then along came the product team...
<br>
### "__Can you guys create a user select that__
### __is inline and doesn't use a dropdown?__"
<br>
### - Product Manager X

---

<!-- .slide: data-background-image="http://i.imgur.com/lEV7M.gif" -->
#ARRGGGHHH!!!!
#Fucking Product Department!!!!

---

<!-- .slide: data-background-image="http://i.imgur.com/ib5GD.gif" -->
#No
##It's your own damn fault

---

## From Phleghm to BEM

```sass
// Ewww
.userSelect-dropdown li {
	//Style list items in the dropdown
}

// Brrrrap!
.userSelect-listItem {
	//Style list items ANYWHERE I WANT! :D
}
```

---

## OOCSS concept:
#Separation Of Layout from Components

---

```
.saleItem {
	float: left;
	width: 25%;
	background-color: $featureBG;
	border: 1px solid $borderColor;
	@include border-radius(3px);
}
```

```
<div class="saleItem">
	<!-- Something -->
</div>

<div class="saleItem">
	<!-- Something -->
</div>

<!-- ... -->
```

---

##This looks better!

```
.saleItem {
	background-color: $featureBG;
	border: 1px solid $borderColor;
	@include border-radius(3px);
}

.grid-quarter {
	float: left;
	width: 25%;
}
```

```
<div class="grid-quarter">
	<div class="saleItem"> <!-- ... --> </div>
</div>
<div class="grid-quarter">
	<div class="saleItem"> <!-- ... --> </div>
</div>

<!-- ... -->
```

---

```
<div class="grid-half">
	<div class="saleItem"> ... </div>
</div>
<div class="grid-half">
	<div class="saleItem"> ... </div>
</div>
<div class="grid-quarter">
	<div class="saleItem"> ... </div>
</div>
<div class="grid-quarter">
	<div class="saleItem"> ... </div>
</div>
```

---

## Remove Context from your Components

---

## jQuery Soup

```
$('.class').click(function(){ 
	/* userAction */ 
});

$('.form').submit(function(){ 
	/* post and react to submission */ 
});

$('.button').click(function(){ 
	/* validate */ 
});

$('.profileImg').hover(function(){ 
	/* show tooltip, display controls */ 
});
```

---

## Backbone

```
var MyForm = Backbone.View.extend({
	events: {
		'submit .form': "formSubmission",
		'click .button': "validate"
	},
	"formSubmission": function(){ 
		/* post and react to submission */ 
	},
	"validate": function(){ 
		/* validate */ 
	},
});

var ProfileImage = Backbone.View.extend({
	events: {
		'click .class': "userAction",
		'hover .profileImg': "displayControls"
	},
	"displayControls": function(){ 
		/* show tooltip, display controls */ 
	},
	"userAction": function(){ 
		/* userAction */ 
	}
});
```

---

## Separate declaration from invocation 
<br>
```
require([ 'myForm' ], function( MyForm ) {
	new MyForm({ el: "#myForm" });
});
```

---

<!-- .slide: data-background-image="/images/BG/rapids.jpg" -->
# <del>Communication</del>
<br>
# <del>Modularity</del>
<br>
# Technical Debt
