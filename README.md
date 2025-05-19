# Ex.08 Design of Interactive Image Gallery
## Date:19.05.2025

Name: Ravikrishnamoorthy D

Register No: 212224040271

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
  <title>Basketball Image Gallery</title>
  <style>
    body {
      background-color: #121212;
      color: white;
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      padding: 20px;
      text-align: center;
    }

    h1 {
      color:whitefacc15;
      margin-bottom: 10px;
    }

    .gallery-container {
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    .main-image {
      width: 600px;
      height: 350px;
      object-fit: cover;
      border: 5px solid orange;
      border-radius: 10px;
      margin-bottom: 15px;
      transition: transform 0.3s;
    }

    .main-image:hover {
      transform: scale(1.02);
    }

    .caption {
      margin-bottom: 25px;
      font-size: 18px;
      font-style: italic;
      color: #ccc;
    }

    .thumbnails {
      display: flex;
      gap: 15px;
      flex-wrap: wrap;
      justify-content: center;
    }

    .thumbnails img {
      width: 100px;
      height: 60px;
      object-fit: cover;
      border: 2px solid #333;
      border-radius: 5px;
      cursor: pointer;
      transition: transform 0.2s, border 0.2s;
    }

    .thumbnails img:hover {
      transform: scale(1.1);
      border-color:orange;
    }

    
  </style>
</head>
<body>

  <h1>Basketball Moments Gallery 🏀</h1>

  <div class="gallery-container">
    <img src="download.jpeg" class="main-image" id="mainImage" alt="Main Image">
    <div class="caption" id="caption">Basketball Court</div>

    <div class="thumbnails">
      <img src="download.jpeg" alt="Basketball Court" onclick="changeImage(this, 'Basketball Court')">
      <img src="chefcurry.jpeg" alt="Chef Curry" onclick="changeImage(this, 'Chef Curry')">
      <img src="james.jpeg" alt="King James" onclick="changeImage(this, 'King James')">
      <img src="kb.jpeg" alt="Kobe Bryant" onclick="changeImage(this, 'Kobe Bryant')">
      <img src="mj.jpeg" alt="michael jordan" onclick="changeImage(this, 'Michael Jordan')">
    </div>
  </div>

  <p style="text-align: center; margin-top: 20px;">
 <br> <h3><strong>Name: Ravikrishnamoorthy D</strong></h3>   <h3><strong>Register No: 212224040271</strong></h3>
</p>


  <script>
    function changeImage(img, captionText) {
      document.getElementById('mainImage').src = img.src;
      document.getElementById('caption').textContent = captionText;
    }
  </script>

</body>
</html>

```
## OUTPUT:

![Screenshot (287)](https://github.com/user-attachments/assets/2a444b02-b795-4b2a-927f-bccd7362b1a2)


## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
