Grid notes:
02/15/2025
See examples: CSS Grid vs Flexbox
  [CSS Grid vs Flexbox Example 1 ](http://127.0.0.1:5500/10.0%20Display%20Grid/example.html)

  [CSS Grid vs Flexbox Example 2 ](https://appbrewery.github.io/grid-vs-flexbox/)


In this exercise: I reviewed my code with some help from AI 

There are several issues with your code that are preventing your chessboard from displaying correctly in the browser:

### **Issues:**
1. **Grid is not structured correctly**  
   - You only defined `grid-template-columns: 100px; grid-template-rows: 100px;`, which means the grid only has a **single column and single row**.
   - To create an 8x8 chessboard, you need `grid-template-columns: repeat(8, 100px);` and `grid-template-rows: repeat(8, 100px);`.

2. **Squares are missing dimensions**  
   - You need to set `width: 100px; height: 100px;` for `.white` and `.black` to make them visible.

3. **Incorrect `color` property**  
   - You're using `color: #f0d9b5;` and `color: #b58863;`, which only changes the **text color**.
   - You should use `background-color: #f0d9b5;` and `background-color: #b58863;` instead.

### **Fixed Code:**
```html
<!DOCTYPE html>
<html>

<head>
  <title>Chessboard</title>
  <style>
    /* Chessboard container */
    .container {
      display: grid;
      grid-template-columns: repeat(8, 100px);
      grid-template-rows: repeat(8, 100px);
    }

    /* Chessboard squares */
    .white, .black {
      width: 100px;
      height: 100px;
    }

    .white {
      background-color: #f0d9b5;
    }

    .black {
      background-color: #b58863;
    }
  </style>
</head>

<body>
  <div class="container">
    <!-- 8x8 Grid of alternating white and black squares -->
    <!-- Row 1 -->
    <div class="white"></div><div class="black"></div><div class="white"></div><div class="black"></div>
    <div class="white"></div><div class="black"></div><div class="white"></div><div class="black"></div>

    <!-- Row 2 -->
    <div class="black"></div><div class="white"></div><div class="black"></div><div class="white"></div>
    <div class="black"></div><div class="white"></div><div class="black"></div><div class="white"></div>

    <!-- Row 3 -->
    <div class="white"></div><div class="black"></div><div class="white"></div><div class="black"></div>
    <div class="white"></div><div class="black"></div><div class="white"></div><div class="black"></div>

    <!-- Row 4 -->
    <div class="black"></div><div class="white"></div><div class="black"></div><div class="white"></div>
    <div class="black"></div><div class="white"></div><div class="black"></div><div class="white"></div>

    <!-- Row 5 -->
    <div class="white"></div><div class="black"></div><div class="white"></div><div class="black"></div>
    <div class="white"></div><div class="black"></div><div class="white"></div><div class="black"></div>

    <!-- Row 6 -->
    <div class="black"></div><div class="white"></div><div class="black"></div><div class="white"></div>
    <div class="black"></div><div class="white"></div><div class="black"></div><div class="white"></div>

    <!-- Row 7 -->
    <div class="white"></div><div class="black"></div><div class="white"></div><div class="black"></div>
    <div class="white"></div><div class="black"></div><div class="white"></div><div class="black"></div>

    <!-- Row 8 -->
    <div class="black"></div><div class="white"></div><div class="black"></div><div class="white"></div>
    <div class="black"></div><div class="white"></div><div class="black"></div><div class="white"></div>
  </div>
</body>

</html>
```

### **What I Fixed:**
✅ Added `grid-template-columns: repeat(8, 100px);` to create an 8-column layout.  
✅ Added `grid-template-rows: repeat(8, 100px);` for an 8-row layout.  
✅ Set `width: 100px; height: 100px;` to make squares visible.  
✅ Changed `color` to `background-color` so squares have the correct colors.  
✅ Corrected the pattern to alternate black and white squares properly.  

Now, this will display a **proper chessboard** in your browser! 🏁 Let me know if you have any other questions. 🚀


See code from lesson 10.0 Display Grid 
<!DOCTYPE html>
<html>

<head>
  <title>Chessboard</title>
  <style>
    /* Write your code here */
    /* Each square should be 100px by 100px */
    /* My colours for white: #f0d9b5, black: #b58863 */
.container {
  display: grid;
  grid-template-columns: repeat(8, 100px);
  grid-template-rows: repeat(8, 100px);
}

.white, .black {
  width: 100px;
  height: 100px;
}

.white {
background-color: #f0d9b5;
}
.black {
background-color: #b58863;
}


  </style>
</head>

<body>
  <div class="container">
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
    <div class="black"></div>
    <div class="white"></div>
  </div>
</body>

</html>