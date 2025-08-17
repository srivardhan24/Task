<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Gallery</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="gallery">
        <h1>Image Gallery</h1>
        <div class="thumbnails">
            <img src="image1.jpg" alt="Image 1" onclick="showImage('image1.jpg')">
            <img src="image2.jpg" alt="Image 2" onclick="showImage('image2.jpg')">
            <img src="image3.jpg" alt="Image 3" onclick="showImage('image3.jpg')">
        </div>
        <div class="full-image">
            <img id="fullImage" src="" alt="Full Image">
        </div>
    </div>
    <script src="script.js"></script>
</body>
</html>


.gallery {
    width: 80%;
    margin: 50px auto;
    text-align: center;
}

.thumbnails {
    display: flex;
    justify-content: center;
    gap: 10px;
    margin-bottom: 20px;
}

.thumbnails img {
    width: 100px;
    height: 100px;
    object-fit: cover;
    cursor: pointer;
    border: 2px solid #ccc;
    border-radius: 10px;
}

.thumbnails img:hover {
    border-color: #aaa;
}

.full-image img {
    max-width: 100%;
    height: auto;
    border: 2px solid #ccc;
    border-radius: 
    }
    
function showImage(imageSrc) {
    document.getElementById('fullImage').src = imageSrc;
}
