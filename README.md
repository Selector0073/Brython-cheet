# Paste this code to import brython: 
```
<head>
  <script src="/src/brython.js"></script>
  <script src="/src/brython_stdlib.js"></script>
</head>

<body>
  <script type="text/python" id="myscript">
    from browser import document, alert, console, window, timer
    --BRYTHON CODE--
  </script>
```

# Commands:
button that hides the box
```
<button id="toggle_btn">hide</button>

<div id="mybox"><img src="https://cdn-icons-png.flaticon.com/512/2175/2175188.png" alt="1"> <p>img</p></div>

script:

def toggle(event):
  box = document["mybox"] //all with id mybox is box element
  if box.style.display == "none": //if box is show > block
    box.style.display = "block"
  else:
    box.style.display = "none"

  document["toggle_btn"].bind("click", toggle) //id toggle_btn activate toggle function when click
```
