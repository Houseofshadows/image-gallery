# image-gallery
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Image Gallery</title>
    <style>
        .gallery {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            padding: 20px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .gallery-item {
            flex: 1 1 300px;
            position: relative;
            overflow: hidden;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            transition: transform 0.3s ease;
        }

        .gallery-item:hover {
            transform: scale(1.03);
        }

        .gallery-item img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            display: block;
        }

        .gallery-caption {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background: rgba(0,0,0,0.7);
            color: white;
            padding: 10px;
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        .gallery-item:hover .gallery-caption {
            opacity: 1;
        }
    </style>
</head>
<body>
    <div class="gallery">
        <div class="gallery-item">
            <img src="https://images.unsplash.com/photo-1469474968028-56623f02e42e" alt="Nature Landscape">
            <div class="gallery-caption">Beautiful Landscape</div>
        </div>
        <div class="gallery-item">
            <img src="https://images.unsplash.com/photo-1477959858617-67f85cf4f1df" alt="City Skyline">
            <div class="gallery-caption">City Life</div>
        </div>
        <div class="gallery-item">
            <img src="https://images.unsplash.com/photo-1472214103451-9374bd1c798e" alt="Forest">
            <div class="gallery-caption">Nature's Beauty</div>
        </div>
        <div class="gallery-item">
            <img src="https://images.unsplash.com/photo-1486299267070-83823f5448dd" alt="Architecture">
            <div class="gallery-caption">Urban Architecture</div>
        </div>
        <div class="gallery-item">
            <img src="https://images.unsplash.com/photo-1495616811223-4d98c6e9c869" alt="Sunset">
            <div class="gallery-caption">Sunset View</div>
        </div>
        <div class="gallery-item">
            <img src="https://images.unsplash.com/photo-1464822759023-fed622ff2c3b" alt="Mountains">
            <div class="gallery-caption">Mountain Range</div>
        </div>
    </div>
</body>
</html>

