<!-- .slide: data-background-image="/images/BG/communication.jpg" -->
# Communication and Collaboration

---

## Developer - Developer

## Developer - Designer

## Designer - QA

---

## Learning Curve

## Inefficiency

## Difficult to Test

---


## "If everyone is moving forward together, then success takes care of itself."
<br>
### Henry Ford

---

<!-- .slide: data-background-image="/images/BG/library.jpg" -->
# Pattern Library

---

<!-- .slide: data-background-image="/images/BG/playground.jpg" -->
## Playground

---

# "What are the classes for --- again?"
<br>
### - Everyone

---

<!-- .slide: data-background-image="/images/BG/red-panda.JPG" -->
# Living Style Guide
<br>
### Inspired by Twitter Bootstrap, we wanted 
### a resource for developers where they  
### could find code examples to reuse  
### components

---

## Self-documenting

```
<div class="codeExample">
	<div class="panel panel--placeholder">
		<h3>This is a placeholder</h3>
		<p>Hmmmm, what could possiply be placed here?</p>
	</div>
</div>
```

---

## Result + Code

!["Website"](/images/pattern.jpg)

---

<!-- .slide: data-background-image="/images/BG/tablet.jpg" -->
# BEM

---

## Block
## Element
## Modifier

---

!["Website"](/images/BEM/site.png)

---

!["Website"](/images/BEM/head-marked.png)
##These are the _blocks_

---

!["Website"](/images/BEM/search-block-marked.png)

---

<!-- .slide: data-background-image="http://4.bp.blogspot.com/-KeSYNRBVcug/T65blLQr6PI/AAAAAAAABJs/OyiLgpH2YRs/s200/troy-and-abed-pointing.gif" -->

---

#Blocks

```sass
// Block
.achieversForm {
	@include inline-block();
	border: 1px solid $formBorderColor;
	@include border-radius(3px);
	padding 2px 5px;
}

```

---

#Elements
```sass

// Element
.achieversForm-input {
	max-width: 500px;
	border: 1px solid $formFieldBorder;
}
```

---

#Modifiers
```sass
// State/Modifiers

.achieversForm--emphasized {
	background-color: $chartreuse;
}

.achieversForm--disabled {
	background-color: $disabledFormBG;
	border-style: dashed;
}

.achieversForm-input--error {
	border-color: $errorColor;
	background-color: $errorColorBG;
}
```

---

<!-- .slide: data-background-image="/images/BG/rapids.jpg" -->
# <del>Communication</del>
<br>
#Modularity
<br>
# Technical Debt
