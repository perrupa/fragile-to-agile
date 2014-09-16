# Step 1
Preprocessor
	- Sass/Less/Stylus/etc
	- minification
	- Absolutely 0 effort

# Step 2
Pattern Library
	- Tell story of Design owners -> Dev owners
	- Inside your platform
	- Documentation for co-workers/developers
	
# Step 3
Specificity
	- Don't start wars!

# Step 4
OOCSS - decouple css from html (no element selectors/nesting)
	- because we only ever use 1 class...

# Step 5
OOCSS - Separate layout from content
	- make all blocks/components *block* or *inline block*
	- use a grid system

# Step 6
OOCSS - Helper classes for layout
	- floats/clearfix, positioning, text-align
	- media object

# Step 7
Context
	- Remove any context from all components
	- clear floats, no positioning etc.

# Step 8
BEM
	- Decide on a naming convention/methodology
	- helps you enforce 1 class selectors
	- Sass makes combining separate, organized files easy

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

