# Styling Options for Different Elements

### In this section, we'll explore various styling options for different elements to enhance the appearance of your first website. 
### Before we start, in VS Code make a new document and call it styles.css this is where we will write the css styling. To import styles.css add:
```
  <link rel="stylesheet" href="styles.css">
```
### Under the ```<head>``` section of your HTML document.

# 3.1 Nav Bar Styling 
## Old:
```
<div class="nav-button">
  <span></span>
  <span></span>
  <span></span>
</div>

<nav class="nav-menu">
  <ul>
    <li><a href="#home">Home</a></li>
    <li><a href="#about">About</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>
```
## New:
```   
   <div class="nav-button">Menu</div>
    <nav class="nav-menu">
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>
```
### In this modified version, we wrapped the navigation bar (navbar) and the nav button together inside a common container (a ```<div>``` element with the class nav-button). By doing this, we can apply styling to the container to position it as a button and trigger the drop-up effect for the navigation menu.
```
    <style>
        /* CSS for the nav button */
.nav-button {
  position: fixed;
  color: #f5f9e9;
  background-color: #1e212b;
  border-style: solid;
  border-color: #9e2b25;
  bottom: 0;
  left: 0px;
  width: 125px;
  height: 32px;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
  cursor: pointer;
  z-index: 9999;
}

.nav-button span {
  width: 100%;
  height: 3px;
  background-color: #1e212b;
  transition: all 0.2s ease;
}

/* CSS for the nav menu */
.nav-menu {
  position: fixed;
  bottom: 0;
  left: 0;
  width: 125px;
  background-color: #1e212b;
  border: solid #9e2b25;
  padding: 10px 0;
  padding-bottom: 10;
  transform: translateY(100%);
  transition: all 0.25s ease;
}

.nav-menu ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

.nav-menu li {
  text-align: center;
  padding: 10px 0;
}

.nav-menu a {
  text-decoration: none;
  color: #f5f9e9;
  display: block;
  transition: color 0.2s ease;
}

.nav-menu a:hover {
  color: #9e2b25;
}

/* Show/hide nav menu on hover */
.nav-button:hover + .nav-menu, .nav-menu:hover {
  transform: translateY(-25%);
}
    </style>
</head>
<body>


    <div class="nav-button">Menu</div>
    <nav class="nav-menu">
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>
```
## CSS for the .nav-button (the Nav Button):
position: fixed;: It positions the nav button relative to the viewport, so it stays fixed on the screen even when the user scrolls.
color: #f5f9e9;: Sets the text color to a light color (almost white).
background-color: #1e212b;: Defines the background color of the nav button to a dark color.
border-style: solid;: Sets the border style to "solid".
border-color: #9e2b25;: Specifies the border color for the nav button.
bottom: 0;: Places the nav button at the bottom of the screen.
left: 0px;: Aligns the nav button to the left side of the screen, with no margin from the left edge.
width: 125px;: Sets the width of the nav button to 125 pixels.
height: 32px;: Sets the height of the nav button to 32 pixels.
display: flex;: Uses flexbox to align the content of the nav button.
flex-direction: column;: Arranges the content in a column (vertically stacked).
justify-content: space-around;: Adds space evenly around the child elements, vertically centering them.
align-items: center;: Horizontally centers the child elements.
cursor: pointer;: Changes the cursor to a pointer when hovering over the nav button, indicating it's clickable.
z-index: 9999;: Sets a high z-index to ensure the nav button is displayed above other elements on the page.

## CSS for the .nav-button span (the Lines Inside the Nav Button):
width: 100%;: Makes the lines occupy the entire width of the nav button.
height: 3px;: Sets the height of the lines to 3 pixels.
background-color: #1e212b;: Sets the color of the lines to match the nav button's background color.
transition: all 0.2s ease;: Adds a smooth transition effect to the lines when they change appearance.

## CSS for the .nav-menu (the Navigation Menu):
position: fixed;: Positions the menu relative to the viewport, similar to the nav button.
width: 125px;: Sets the width of the menu to 125 pixels, matching the nav button's width.
background-color: #1e212b;: Sets the background color of the menu to a dark color, similar to the nav button.
border: solid #9e2b25;: Adds a solid border around the menu with the same color as the nav button's border.
padding: 10px 0;: Adds 10 pixels of padding at the top and bottom of the menu.
padding-bottom: 10;: Fixes a typo in the padding-bottom property (should be 10px instead of 10).
transform: translateY(100%);: Moves the menu 100% (its own height) downward, hiding it below the screen.
transition: all 0.25s ease;: Adds a smooth transition effect to the menu when it appears.

## CSS for the .nav-menu ul (the List Inside the Menu):
list-style: none;: Removes the default list bullet points.
padding: 0;: Removes any default padding from the list.

## CSS for the .nav-menu li (the List Items Inside the Menu):
text-align: center;: Centers the text inside the list items.
padding: 10px 0;: Adds 10 pixels of padding at the top and bottom of each list item.

## CSS for the .nav-menu a (the Links Inside the Menu):
text-decoration: none;: Removes underlines from the links.
color: #f5f9e9;: Sets the color of the links to a light color (almost white).
display: block;: Makes the links fill the entire width of the list items.
transition: color 0.2s ease;: Adds a smooth transition effect to the link text when it changes color on hover.

## CSS for the Hover Effect to Show/Hide the Menu:
.nav-button:hover + .nav-menu, .nav-menu:hover: Targets the .nav-menu when the .nav-button is hovered or when the .nav-menu itself is hovered.
transform: translateY(-25%);: Moves the menu 25% (its own height) upward, revealing it when the button is hovered over.
