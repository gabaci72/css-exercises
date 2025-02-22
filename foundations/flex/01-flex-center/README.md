# CENTER THIS DIV
This one is simple, but it's something that you'll want to do ALL THE TIME.  Might as well get it out of the way now.

All you need to do is center the red div inside the blue container.

## Desired Outcome
![outcome](./desired-outcome.png)

### Self Check
- Is the red div centered?
- Did you _only_ use flexbox to center it?

### Solutions:
```css
.container {
      display: flex; /* Enable flexbox on the .container */
      align-items: center; /* Center the child element vertically */
      justify-content: center; /* Center the child element horizontally */
           }   
```