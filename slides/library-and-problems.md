# CSS Best Practices 

---

## We want to be able to build as quickly as possible

---

# Lego is more agile than clay
<br>
### Leverage your pattern library

---

# Problem #1 encountered
<br>
### Tight coupling / Context Dependency

---

# Specificity
<br>
### Let me explain.

---

## There are 4 types of specificity and one 'trump'

- elements ( `li` )

- classes ( `.listItem` )

- IDs ( `#listItem` )

- inline ( `<li style="font-weight: bold;">` )

- important! ( `font-weight: bold !important` )

---

# Quiz

```css
#navBar .dropdownMenu li a .selected #currentUser .elem { /* ... */ }
.navBar #menu .nestedItem li > a em .focussed::last-child { /* ... */ }
```

---


# Quiz #2

```css
.navBar .listItem { /* ... */ }
.floatRight { /* ... */ }
```

---

## User List

```
.userList li { /* ... */ }
.userList img { /* ... */ }
```

<pre><code>
<ul class="userList">
	<li><img src="/dick.jpg" alt=""> Dick</li>
	<li><img src="/jane.jpg" alt=""> Jane</li>
</ul>
</code></pre>

---

## Add an inline-list
 
```
.inlineList span,
.userList li { /* ... */ }

.inlineList img,
.userList img { /* ... */ }
```

<pre><code>
<div class="inlineList">
	<span><img src="/dick.jpg" alt=""> Dick</span>
	<span><img src="/jane.jpg" alt=""> Jane</span>
</div>
</code></pre>

---

## Modify a style

```
.inlineList span,
.userList li { /* ... */ }

/* needs specifity... */ 
.userList li.promoted { /* ... */ }

.inlineList img,
.userList img { /* ... */ }
```

<pre><code>
<div class="inlineList">
	<span><img src="/dick.jpg" alt=""> Dick</span>
	<span class="promoted"><img src="/jane.jpg" alt=""> Jane</span>
</div>
</code></pre>

---

# This was problem #2
<br>
### We needed a solution...