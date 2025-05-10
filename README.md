# Ex.08 Design of Interactive Image Gallery
## Date:

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
<html>

<head>
    <title> MY LIFESTYLE</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #963950;
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
            margin: 20px;
            width: 200px;
            height: auto;
            cursor: pointer;
            border-radius: 15px;
            border: 2px solid #252727;
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
            width: 80%;
            height: 80%;
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

        .back {
            background-color: rgb(132, 34, 120);
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

<body class="back">

    <h1 align="center" style="font-family: Georgia, 'Times New Roman', Times, serif;color: rgb(85, 18, 56);">
        MY LIFESTYLE 
    Shravani M 212224230263</h1>
    <div class="gallery">
        <br><br><br>
        <img src="paris.jpg" alt="Image 1" class="gallery-item" onclick="openModal(this)">
        <img src="outfit.jpg" alt="Image 2" class="gallery-item" onclick="openModal(this)">
        <img src="skincare.jpg" alt="Image 3" class="gallery-item" onclick="openModal(this)">
        <img src="travel.jpg" alt="Image 4" class="gallery-item" onclick="openModal(this)">
        <img src="house.jpg" alt="Image 5" class="gallery-item" onclick="openModal(this)">
        <img src="car.jpg" alt="Image 5" class="gallery-item" onclick="openModal(this)">
    </div>
    <div id="imageModal" class="modal" onclick="closeModal()">
        <span class="close">&times;</span>
        <img class="modal-content" id="modalImage">
    </div>

</body>

</html>
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/01ccee79-da73-4782-8af8-38c394372d9a)

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
