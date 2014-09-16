# Modular Javascript

---

# Step 9
Pattern Library 2: Electric Boogaloo
	- Sandbox for component development
	- Isolated dev environment
		- know all dependencies

# Step 10
JS - jQuery to Backbone
	- Give your JS some structure

# Step 11
JS - Separate declaration from invocation 
	- JS reuse no longer a problem
	- Build System

# Step 12
JS Separate behavior from style
	- classnames vs attributes
	".js-behavior" vs "[pfa-behavior]"

# Step 13
JS events over callbacks
	- No one needs to be listening.

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
		'click .class': "userAction"
		'submit .form': "formSubmission"
		'click .button': "validate"
		'hover .profileImg': "displayControls"
	},
	"userAction": function(){ 
		/* userAction */ 
	},
	"formSubmission": function(){ 
		/* post and react to submission */ 
	},
	"validate": function(){ 
		/* validate */ 
	},
	"displayControls": function(){ 
		/* show tooltip, display controls */ 
	},
});

new MyForm({ el: "#myForm" });
```
