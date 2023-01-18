

> Overall Bootstrap

If you are working with mobile devices, make sure and add this at the top of the page inside the head tag. It sets the width of the page to follow the screen-width of the device.

	<meta name="viewport" content="width=device-width, initial-scale=1">

When using bootstrap you need to put things in containers. There's 

	.container - responsive and fixed-width
	.container-fluid - spans the entire viewport

The .container class width will change based on the screen size so there is always margins each side except for when the screen is super tiny, and then it fills the whole screen. 

If you want to pad the top and bottom, then you just need to add some "padding-bottom" and "padding-top" as follows:
	
	<div class="container pb-5 pt-5" style="background-color: #5b9aeb">

Or if you want to pad all sides and add some margins between elements

	<div class="container p-5 my-5 bg-dark text-white">

> Bootstrap Grid System

Bootstrap 5 chops up the screen into twelve segments that you can use. You can merge and groups these however you need to create the vertically sized elements that you need. 

The responsive part of it is that the columns will stack up on the scren at a specified size. They won't just keep shrinking and cramming content together. So waht this means is that at 576px, the columns will no longer sit next to each other on the screen but will suddenly stack on top of each other.

	col - sm - 3 == "make a column" , "that stacks at 576px" , that's 3/12 wide

	  <div class="row">
	    <div class="col-sm-3 p-3 bg-primary text-white">.col</div>
	    <div class="col-sm-3 p-3 bg-dark text-white">.col</div>
	    <div class="col-sm-3 p-3 bg-primary text-white">.col</div>
	    <div class="col-sm-3 p-3 bg-dark text-white">.col</div>
	  </div>

If you don't put an col-(x/12) value on the end, it sizes them automatically.


---

## Note

An alternative to Bootstrap is W3.CSS
https://www.w3schools.com/w3css/default.asp


---


# Bookmark

https://www.w3schools.com/bootstrap5/bootstrap_typography.php



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
