
```css

/* ========== CHALLENGE 1 ========== //
//
// Use the type selector to: 
// 1. Set the image width to 200px
// 2. Set the list style of <ul> to none
// 3. Add a dark red color to the <h1>
//
*/
img {
    width: 200px;  /* Sets the image width to 200px */
}
ul {
    list-style: none;  /* Sets list style to none */
}
h1 {
    color: darkred;  /* Sets h1 to dark red */
}

/* ========== CHALLENGE 2 ========== //
//
// 1. Style the recipe card so that it has a 
//      -- background color of #FFFAFA
//      -- text is aligned center
// 2. Set text inside recipe-content to align left
//
*/

.recipe-card {
    width: 400px;
    background-color: #FFFAFA;  /* Sets the background color of the recipe card */
    text-align: center;  /* Aligns the text in the recipe card to the center */
}

.recipe-content {
    text-align: left;  /* Aligns the text inside recipe-content to the left */
}

/* ========== CHALLENGE 3 ========== //
//
// 1. Change <h2> elements within a <ul> and <li> to be 16px
// 2. Update recipe card link styles, set:
//      -- background color to #fc9400
//      -- text color to white
//      -- remove underline
*/

.recipe-card h2,
.recipe-card li h2 {
    font-size: 16px;  /* Challenge part 1: Sets the <h2> size to 16px inside <ul> or <li> within recipe-card */
}

.recipe-card a {
    background-color: #fc9400;  /* Sets the background color */
    color: white;  /* Sets the text color */
    text-decoration: none;  /* Removes the underline from the text */
}

```