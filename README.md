# Ex.08 Design of Interactive Image Gallery
## Date

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Interactive Image Gallery</title>
  <style>
    body {
  font-family: Arial, sans-serif;
  background-color: #f3f3f3;
  margin: 0;
  padding: 0;
}

.gallery {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  padding: 20px;
  justify-content: center;
}

.gallery-item {
  width: 200px;
  height: auto;
  cursor: pointer;
  border: 2px solid #842b2b;
  transition: transform 0.01s;
}

.gallery-item:hover {
  transform: scale(1.2);
}

.modal {
  display: none;
  position: fixed;
  z-index: 1;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.8);
  justify-content: center;
  align-items: center;
}

.modal-content {
  max-width: 80%;
  max-height: 80%;
}

.close {
  position: absolute;
  top: 20px;
  right: 30px;
  font-size: 30px;
  color: white;
  cursor: pointer;
}

  </style>
  <script>
    function openModal(image) {
  const modal = document.getElementById('imageModal');
  const modalImg = document.getElementById('modalImage');
  
  modal.style.display = "flex";
  modalImg.src = image.src;
}
function closeModal() {
  const modal = document.getElementById('imageModal');
  modal.style.display = "none";
}
  </script>
</head>
<body background="https://static.vecteezy.com/system/resources/previews/038/811/269/non_2x/ai-generated-beautiful-background-for-flower-shop-advertising-free-photo.jpeg"></body>

 <h1 align="center" style="font-family: Georgia, 'Times New Roman', Times, serif;color: rgb(132, 132, 224);">Interactive Image Gallery</h1>
  <div class="gallery">
    <br><br><br>
    <img src="/static/eye.jpg" alt="Image 1" class="gallery-item" onclick="openModal(this)">
    <img src="/static\dock.jpg" alt="Image 2" class="gallery-item" onclick="openModal(this)">
    <img src="/static\mona lisa.jpg" alt="Image 3" class="gallery-item" onclick="openModal(this)">
    <img src="/static\tree.jpg" alt="Image 4" class="gallery-item" onclick="openModal(this)">
    <img src="/static\art.jpg" alt="Image 5" class="gallery-item" onclick="openModal(this)">    
    <img src="/static\mountain.jpg" alt="Image 6" class="gallery-item" onclick="openModal(this)">    
    <img src="/static\sun.jpg" alt="Image 7" class="gallery-item" onclick="openModal(this)">    
  </div>
  <div id="imageModal" class="modal" onclick="closeModal()">
    <span class="close">&times;</span>
    <img class="modal-content" id="modalImage">
  </div>

</body>
</html>
```

## OUTPUT:
![alt text](<Screenshot 2024-12-21 142036.png>)

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
