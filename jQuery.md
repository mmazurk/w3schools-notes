

Run when the window is done loading

	$(document).ready(function(){

	  // jQuery methods go here...

	});

> Selecting Stuff

What is this man doing? For answers go to: 
https://www.w3schools.com/jquery/jquery_selectors.asp

	$("*")
	$(this) 
	$("p.intro") 
	$("p:first") 
	$("ul li:first") 	
	$("ul li:first-child") 	
	$("[href]") 
	$("a[target='_blank']") 	
	$("a[target!='_blank']") 	
	$(":button") 	
	$("tr:even") 
	$("tr:odd") 

The typical way to make an event happen is

	$("p").click(function () {
		$(this).hide();
	})

	$("p").on("click", function () {
		$(this).hide();
		})

Although we learned to use "on" at Springboard, this is typically used to attach multiple event handlers to a single thing. And wow, you do this with an object. In this case there are three keys with functions as values (whoa). 

	$("p").on({
	  mouseenter: function(){
	    $(this).css("background-color", "lightgray");
	  },
	  mouseleave: function(){
	    $(this).css("background-color", "lightblue");
	  },
	  click: function(){
	    $(this).css("background-color", "yellow");
	  }
	});

When thinking of events, typically you have things like: Mouse Events, Keyboard Events, Form Events, and Document / Window events. You can look up what these are! 

You can also hide and show elements rather than just modifying the styles!

	$("p").hide(speed, callback);
	$("p").show(speed, callback);

In fact, there's an entire list of jQuery effects methods here: https://www.w3schools.com/jquery/jquery_ref_effects.asp

Some of the more popular methods include

	fadeIn()
	fadeOut()
	fadeToggle()
	fadeTo()

# Bookmark

https://www.w3schools.com/jquery/jquery_fade.asp



---

## CDNs for all of your Pages

> Styles

	<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css">
	<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.11.2/css/all.min.css">

> Scripts

	<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js">
	<script src="https://unpkg.com/jquery"></script>
	<script src="https://unpkg.com/axios/dist/axios.js"></script>
	<script src="https://unpkg.com/lodash"></script>

---

