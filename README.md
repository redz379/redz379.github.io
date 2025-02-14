<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Media Gallery</title>
    <style>
        #gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .media {  /* Combined class for both photos and videos */
            margin: 10px;
        }

        img, video {
            max-width: 300px;
            height: auto;
        }
    </style>
</head>
<body>

    <header>
        <h1>My Media Gallery</h1>
    </header>

    <div id="gallery">
        <div class="media">
            <img src="https://github.com/user-attachments/assets/72c2ad80-c62e-4468-88ec-e9c40cb52d4d" alt="A vibrant sunset over a calm ocean.">
        </div>
        <div class="media">
            <img src="https://github.com/user-attachments/assets/2e573fcf-6f71-4ab7-9e10-5211eb849eeb" alt="A playful golden retriever puppy running through a field.">
        </div>
        <div class="media">
            <video controls>
                <source src="YOUR_VIDEO_URL_1.mp4" type="video/mp4">
                <track src="captions1.vtt" kind="captions" label="English captions">  Your browser does not support the video tag.
            </video>
        </div>
        <div class="media">
            <video controls>
                <source src="YOUR_VIDEO_URL_2.mp4" type="video/mp4">
                <track src="captions2.vtt" kind="captions" label="English captions">  Your browser does not support the video tag.
            </video>
        </div>
        </div>

    <footer>
        <p>&copy; <span id="year"></span> My Website</p>
    </footer>

    <script>
        document.getElementById("year").textContent = new Date().getFullYear();
    </script>

</body>
</html>![1000031373](https://github.com/user-attachments/assets/c8c14cb7-0106-438e-90a3-1363743af679)
![1000031382](https://github.com/user-attachments/assets/68503369-d446-45e0-8d53-a20d92a793ac)
![1000031379](https://github.com/user-attachments/assets/cf4fe68e-1c94-4548-8828-9e3e5799d75c)
![1000031385](https://github.com/user-attachments/assets/e53b6d5d-662f-4e02-b501-31d7943c5cbf)
