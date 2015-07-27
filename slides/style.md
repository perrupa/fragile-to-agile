# Style

---

> __"<del>Javascript</del> CSS doesn't suck,__
> 
> __you're just doing it wrong."__
>
> - Douglas Crockford

---

# Preprocess

---

## Compile your CSS

- Sass [http://sass-lang.com](http://sass-lang.com)
- Less [http://lesscss.org](http://lesscss.org)
- Stylus [http://learnboost.github.io/stylus](http://learnboost.github.io/stylus)
- etc...

<br>

Which one doesn't really matter.

---

# Document

---

## Pattern Library

- Document your most common patterns
- Make it dead-simple for others to do the same.

---

## Self-executing and documenting

<pre><code><div class="codeExample">
	<input type="text" class="userSelect">
	<script>
		require(["userSelect"], function( UserSelect ){
			new UserSelect({ el: $(".userSelect") });
		}); // I'll explain this later..
	</script>
</div>
</code></pre>

---

## Now we have a good starting point