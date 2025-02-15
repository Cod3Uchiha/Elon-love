## HTML File

```html
<!DOCTYPE html>
<html>
<head>
  <title>Valentine's Card</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <div class="card">
    <div class="heart-container">
      <div class="heart"></div>
      <div class="heart"></div>
      <div class="heart"></div>
    </div>

    <div class="message">
      <h1>Happy Valentine's Day, Elon!</h1>
      <p>From, Your Secret Admirer</p>
    </div>
  </div>

  <script src="script.js"></script>
</body>
</html>
```

## CSS File

```css
/* Reset styles */

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* Card styles */

.card {
  width: 500px;
  height: 500px;
  margin: auto;
  background-color: #ffffff;
  border: 1px solid #000000;
  border-radius: 10px;
  box-shadow: 5px 5px 5px #000000;
}

/* Heart container styles */

.heart-container {
  width: 200px;
  height: 200px;
  margin: auto;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

/* Heart styles */

.heart {
  width: 50px;
  height: 50px;
  background-color: #ff0000;
  border-radius: 50%;
  position: absolute;
  animation: heart-beat 1s infinite;
}

/* Heart animation */

@keyframes heart-beat {
  0% {
    transform: scale(1);
  }
  50% {
    transform: scale(1.2);
  }
  100% {
    transform: scale(1);
  }
}

/* Message styles */

.message {
  width: 200px;
  height: 100px;
  margin: auto;
  position: absolute;
  bottom: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

/* Message text styles */

h1 {
  font-size: 20px;
  font-weight: bold;
  text-align: center;
}

p {
  font-size: 14px;
  text-align: center;
}
```

## JavaScript File

```javascript
// Get the heart elements
const hearts = document.querySelectorAll(".heart");

// Add an event listener to the hearts
hearts.forEach((heart) => {
  heart.addEventListener("click", () => {
    // Toggle the heart animation
    heart.classList.toggle("heart-beat");
  });
});
```

## Implementation Details

The card is created using a simple HTML structure. The heart animation is achieved using CSS animations. The JavaScript code adds event listeners to the hearts so that they can be toggled on and off when clicked.

## Documentation

The code is well-documented with comments. The CSS animations are documented in the CSS file. The JavaScript code is documented in the JavaScript file.

## Conclusion

This is a simple but effective HTML and CSS Valentine's card for Elon Musk. The card is easy to customize and can be used to express your love for Elon Musk.