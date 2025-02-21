Because the `content-box` value is set to the default value, elements exhibit this behavior even without specifying the `box-sizing: content-box;` property. However, the `content-box` value is the default value, not the initial value. Therefore, elements exhibit this behavior even without specifying the `box-sizing: content-box;` property.

### Default Behavior

By default, all HTML elements exhibit `box-sizing: content-box;` behavior. Therefore, even without specifying the `box-sizing: content-box;` property, the width and height of elements only cover the content.

### Example

Below is an example that shows the behavior of elements in two different cases without specifying the `box-sizing` property and specifying it.

### HTML Code
```html
<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>Box Sizing Example</title>
 <link rel="stylesheet" href="styles.css">
</head>
<body>
 <div class="box default-box">Default Box</div>
 <div class="box content-box">Content Box</div>
 <div class="box border-box">Border Box</div>
</body>
</html>
```

### CSS Code (styles.css)
```css
*{
 outline: 2px solid red;
 box-sizing: border-box; /* This ensures padding and border are included in the element's total width and height */
}

.box {
 width: 200px;
 height: 100px;
 background-color: #3498db;
 border: 5px solid #2980b9;
 padding: 20px;
 margin: 30px;
}

.default-box {
 background-color: #e74c3c;
}

.content-box {
 box-sizing: content-box; /* Default value */
 background-color: #e74c3c;
}

.border-box {
 box-sizing: border-box; /* This setting */
 background-color: #2ecc71;
}
```

### Descriptions

1. **`.default-box`**: This class exhibits the default `content-box` behavior without specifying the `box-sizing` property.
- Width: 200px (content) + 20px (left padding) + 20px (right padding) + 5px (left border) + 5px (right border) = 250px
- Height: 100px (content) + 20px (top padding) + 20px (bottom padding) + 5px (top border) + 5px (bottom border) = 150px

2. **`.content-box`**: This class specifies the `box-sizing: content-box;` property.
- Width: 200px (content) + 20px (left padding) + 20px (right padding) + 5px (left border) + 5px (right border) = 250px

- Height: 100px (content) + 20px (top padding) + 20px (bottom padding) + 5px (top border) + 5px (bottom border) = 150px

3. **`.border-box`**: This class specifies the `box-sizing: border-box;` property.

- Width: 200px (content + padding + border)

- Height: 100px (content + padding + border)

### Visual Description

Open the page and observe the dimensions of the elements. The width and height of the `.default-box` and `.content-box` elements will be larger than the `.border-box` element. To see this difference, observe the borders and padding of the elements.

- **`.default-box`**: Width 250px, Height 150px
- **`.content-box`**: Width 250px, Height 150px
- **`.border-box`**: Width 200px, Height 100px

In this way, you should have a better understanding of the difference between `box-sizing: content-box;` and `box-sizing: border-box;`. The `content-box` value is the default value, not the initial value.