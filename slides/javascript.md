# Modular Javascript

---

# Pattern Library 2:
<br>
### Electric Boogaloo

---

- Sandbox for component development
- Isolated dev environment
	- you know all your dependencies

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

---


# Separate declaration from invocation 
<br>
### JS reuse no longer a problem

---

# Separate behavior from style

---

```
// Can you spot the dependency?
$(".searchArea").click();
```

# Step 13
JS events over callbacks
	- No one needs to be listening.

