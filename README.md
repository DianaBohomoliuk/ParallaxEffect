# ParallaxEffect
Parallax effect for mobile phone using lax.js.
## Setup and usage
1. Add lax.js to your html via CDN
``` 
<script src="https://cdn.jsdelivr.net/npm/lax.js" ></script>
```
2. Initialize the plugin
```
window.onload = function() {
	lax.setup()

	const updateLax = () => {
		lax.update(window.scrollY)
		window.requestAnimationFrame(updateLax)
	}

	window.requestAnimationFrame(updateLax)
}
```
3. Set the screen to the size of mobile phone.
4. Scroll.
