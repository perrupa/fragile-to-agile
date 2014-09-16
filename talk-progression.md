


# Intro

### Start with a messy system

### Add sass/less/stylus

- instant minification
- all future benefits
- add compass/bourbon/etc or polyfiller

### Start documenting patterns/components _ASAP_ in a library

- build new features in your library, so they're documented
- find and remove duplication/similarities

### Time to clean up CSS

- Get some grids.
- Remove context from your styles
	- widths
	- floats
	- positioning
	- etc...

### Pick a naming convention
- BEM is sweet
- Name based on 'behaviour' and/or 'representation'
	- not it's 'contents' or 'appearance'
	- what is big and blue today, may be small and green a year from now.
- Eliminate as much specifity as possible
	- no element or ID selectors
	- Specificity wars are wars (and war is bad)


### Get some OOCSS going on 

- create helper classes for most common css behaviours (paticularly, layout)
	- floats
	- clearfix
	- display/positioning


### Tidy up your JS a bit

- Absolutely avoid mixing script and code.
- jQuery soup -> Backbone views and models
- Separate JS definitions declarations from invocation
- Adopt a build system
