<!-- .slide: data-background-image="/images/BG/messy messy kitchen.jpg" -->
# Technical Debt

---

## Duplicate Code
<br>
## Disorganized Codebase
<br>
## Page Performance

---

## Pre-process your CSS

---

![css](/images/css.jpg)

---

### After pre-processing, our CSS shrunk around 40-45% of its original size

---

## Adopt some sort of build system

---

## SASS to CSS

```
@import "base/foundations";
@import "platform_components";
@import "base/components";
@import "helpers";
@import "base/platform_default";
@import "screen_reader";
```

---

## JS Modules to a JS Package
```
define([
	'views/dialog',
	'dom/components/file_manager/image_manager'
], function( Dialog, ImageManager ) {

	var ImageManagerDialog = Dialog.extend({ /*...*/ })
	
	return ImageManagerDialog;
});
```

---

# Pattern Library
### Beyond the Thunderdome
<br>
<br>
## Documented Patterns
<br>
## Obvious Inconsistencies
<br>
## Removed Duplication of Efforts

---

<!-- .slide: data-background-image="/images/BG/rapids.jpg" -->
# <del>Communication</del>
<br>
# <del>Modularity</del>
<br>
# <del>Technical Debt</del>
