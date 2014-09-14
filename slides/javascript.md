# Modular Javascript

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
