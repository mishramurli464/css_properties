# css_properties

## Box Model Properties
**max-width**: 300px; : Ensures the card doesn't exceed 300px in width.  
**margin: 20px auto;** : Centers the card horizontally and adds 20px of margin above and below.  
**padding: 20px;** : Adds 20px of space inside the card's border.  
**border: 1px solid #ddd;** : Sets a light gray border around the card.  
**border-radius:** 10px; : Rounds the card's corners.  
**box-shadow:** 0 4px 8px rgba(0, 0, 0, 0.1);: Adds a subtle shadow for depth.  
**overflow: hidden;** : Ensures content doesn't overflow outside the card's boundaries.  

## Layout Properties  
**display: block;** : Ensures the image takes up the full width of its container.  
**width: 100%;** : The image is responsive and fits the card's width.  
**height: auto;** : Maintains the image's aspect ratio.  

## Typography Properties  
**font-family:'Arial, sans-serif';** : Sets the font for the card title.  
**font-size: 1.5em;** : Makes the card title larger.  
**color: #333;** : Sets a dark gray color for the title text.  
**margin: 0 0 10px;** : Adds space below the title.  
**font-family: 'Georgia, serif';** : Sets a different font for the card description.  
**font-size: 1em;** : Sets a standard font size for the description.  
**color: #666;** : Sets a lighter gray color for the description text.  
**line-height: 1.6;** : Improves readability by increasing line height.  


## Responsive 
**Design@media (max-width: 600px) { ... }**: Applies styles for screens smaller than 600px.  
**max-width: 90%;** : Ensures the card takes up 90% of the viewport width on small screens .  
**padding: 10px;** : Reduces padding on small screens.  
**font-size: 1.2em;** : Decreases the title's font size for better fit.  
**font-size: 0.9em;** : Decreases the description's font size for better readability on small screens.

## Position property in css  

There are five different position values:
**1)static (default)**  
This is the default value. Elements are positioned according to the normal flow of the document. top, right, bottom, and left properties have no effect.  
```css
.element {
  position: static;
}
```


**2)relative**
The element is positioned relative to its normal position. Using top, right, bottom, or left will move the element from its normal position without affecting the layout of surrounding elements.  

```css
.element {
  position: relative;
  top: 10px;  /* Moves the element 10px down from its normal position */
  left: 20px; /* Moves the element 20px to the right from its normal position */
}
```


**3)absolute**  
The element is positioned relative to its nearest positioned ancestor (an ancestor with a position other than static). If no such ancestor exists, it is positioned relative to the initial containing block (usually the <html> element).  
```css
.container {
  position: relative;
}

.element {
  position: absolute;
  top: 10px;
  right: 20px;
}
```


**4)fixed**  
The element is positioned relative to the browser window and will not move when the page is scrolled.  
```css
.element {
  position: fixed;
  top: 0;
  left: 0;
}
```  
**5)sticky**
The element is positioned based on the user's scroll position. It toggles between relative and fixed, depending on the scroll position. It is treated as relative until its containing block crosses a specified threshold (defined by top, right, bottom, or left), after which it is treated as fixed.  
```css
.element {
  position: sticky;
  top: 0; /* The element will be fixed at the top of the container when scrolled to the top */
}
```

## Display propertyb in css  
**1)block**
An element with display: block takes up the full width available, and each block element starts on a new line.  

**2.) inline**
An element with display: inline does not start on a new line and only takes up as much width as necessary. It cannot have width or height set.  

**3. inline-block**
An element with display: inline-block is like an inline element, but it can have width and height set.

**4. none**
An element with display: none is not displayed at all (it is removed from the document layout).

**5)flex**
An element with display: flex becomes a flex container, enabling a flexible layout with its children (flex items).  

**6. inline-flex**
An element with display: inline-flex behaves like an inline element but its children are laid out using flexbox.

**7. grid**
An element with display: grid becomes a grid container, enabling a grid layout with its children (grid items).

**8. inline-grid**
An element with display: inline-grid behaves like an inline element but its children are laid out using grid layout.




