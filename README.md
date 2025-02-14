

https://github.com/user-attachments/assets/494d4e35-3d02-44d1-920a-c3051be9b31e

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Photo Gallery</title>
    <style>
        body {
            font-family: sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0;
        }
        header {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 1em 0;
        }
        #gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            padding: 20px;
        }
        .photo {
            margin: 10px;
            border: 1px solid #ccc;
            box-shadow: 2px 2px 5px rgba(0,0,0,0.2);
            max-width: 300px;
            height: auto;
        }
        .photo img {
            max-width: 100%;
            height: auto;
            display: block;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 1em 0;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>

    <header>
        <h1>My Photo Gallery</h1>
    </header>

    <div id="gallery">
        <div class="photo">
            <img src="https://github.com/user-attachments/assets/72c2ad80-c62e-4468-88ec-e9c40cb52d4d" alt="Description of image 1">
        </div>
        <div class="photo">
            <img src="https://github.com/user-attachments/assets/2e573fcf-6f71-4ab7-9e10-5211eb849eeb" alt="Description of image 2">
        </div>
        <div class="photo">
            <img src="https://github.com/user-attachments/assets/480defde-0aa2-4c7e-ac28-80805f70bf97" alt="Description of image 3">
        </div>
        <div class="photo">
            <img src="https://github.com/user-attachments/assets/aa95fed2-c193-46bb-9504-0ec1cebaee75" alt="Description of image 4">
        </div>
        <div class="photo">
            <img src="https://github.com/user-attachments/assets/573fa0b0-18aa-4f37-bae9-4f620887e0fa" alt="Description of image 5">
        </div>
    </div>

    <footer>
        <p>&copy; <span id="year"></span> My Website</p>
    </footer>

    <script>
        document.getElementById("year").textContent = new Date().getFullYear();
    </script>

</body>
</html>
</html>
Sure, I can help you update your code to include videos in addition to photos. Below is the updated code to include videos in your gallery.

HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Media Gallery</title>
    <style>
        body {
            font-family: sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0;
        }
        header {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 1em 0;
        }
        #gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            padding: 20px;
        }
        .media {
            margin: 10px;
            border: 1px solid #ccc;
            box-shadow: 2px 2px 5px rgba(0,0,0,0.2);
            max-width: 300px;
            height: auto;
        }
        .media img, .media video {
            max-width: 100%;
            height: auto;
            display: block;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 1em 0;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>

    <header>
        <h1>My Media Gallery</h1>
    </header>

    <div id="gallery">
        <div class="media">
            <img src="https://github.com/user-attachments/assets/72c2ad80-c62e-4468-88ec-e9c40cb52d4d" alt="Description of image 1">
        </div>
        <div class="media">
            <img src="https://github.com/user-attachments/assets/2e573fcf-6f71-4ab7-9e10-5211eb849eeb" alt="Description of image 2">
        </div>
        <div class="media">
            <img src="https://github.com/user-attachments/assets/480defde-0aa2-4c7e-ac28-80805f70bf97" alt="Description of image 3">
        </div>
        <div class="media">
            <img src="https://github.com/user-attachments/assets/aa95fed2-c193-46bb-9504-0ec1cebaee75" alt="Description of image 4">
        </div>
        <div class="media">
            <img src="https://github.com/user-attachments/assets/573fa0b0-18aa-4f37-bae9-4f620887e0fa" alt="Description of image 5">
        </div>
        <div class="media">
            <video controls>
                <source src="https://github.com/user-attachments/assets/video1.mp4" type="video/mp4">
                Your browser does not support the video tag.
            </video>
        </div>
        <div class="media">
            <video controls>
                <source src="https://github.com/user-attachments/assets/video2.mp4" type="video/mp4">
                Your browser does not support the video tag.
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
</html>
 Public code references from 1 repository
This updated HTML includes both images and videos in the gallery. The media class is used for both images and videos to apply consistent styling.

1 reference
How is this
Your HTML code looks good and includes functionality to upload both images and videos. However, keep in mind that the file upload is currently simulated and doesn't actually send files to a server. Here's a slightly refined version to ensure clarity and better practices:

HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>I Love My Girlfriend</title>
    <style>
        body {
            background-color: #f0f0f0;
            background-image: url("heart_background.jpg");
            background-size: cover;
            background-repeat: no-repeat;
            font-family: sans-serif;
            color: #333;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            min-height: 100vh;
        }
        .container {
            background-color: rgba(255, 255, 255, 0.8);
            padding: 20px;
            border-radius: 10px;
            margin-top: 20px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            max-width: 800px;
        }
        h1 {
            color: #e91e63;
            text-align: center;
        }
        p {
            text-align: center;
            line-height: 1.6;
        }
        .upload-section {
            margin-top: 20px;
            text-align: center;
        }
        input[type="file"] {
            margin-bottom: 10px;
        }
        @media (max-width: 600px) {
            .container {
                padding: 10px;
            }
            h1 {
                font-size: 1.5em;
            }
            p {
                font-size: 0.9em;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>I Love My Girlfriend</h1>
        <p>This page is dedicated to the most amazing person in my life. She's kind, beautiful, and makes every day an adventure. I'm so lucky to have her, and I wanted to create a special place to show my appreciation.</p>
        <div class="upload-section">
            <h2>Upload Memories</h2>
            <input type="file" id="imageUpload" name="imageUpload" accept="image/*"> <br>
            <input type="file" id="videoUpload" name="videoUpload" accept="video/*"> <br><br>
            <button onclick="uploadFiles()">Upload</button> <br><br>
            <div id="fileStatus"></div>
        </div>
    </div>

    <script>
        function uploadFiles() {
            const imageUpload = document.getElementById('imageUpload');
            const videoUpload = document.getElementById('videoUpload');
            const fileStatus = document.getElementById('fileStatus');

            const files = [];

            if (imageUpload.files.length > 0) {
                for (const file of imageUpload.files) {
                    files.push(file);
                }
            }

            if (videoUpload.files.length > 0) {
                for (const file of videoUpload.files) {
                    files.push(file);
                }
            }

            if (files.length === 0) {
                fileStatus.textContent = "No files selected.";
                return;
            }

            fileStatus.textContent = "Uploading...";

            setTimeout(() => {
                fileStatus.textContent = "Upload Complete (Simulated)";
                imageUpload.value = '';
                videoUpload.value = '';
            }, 2000);

            // Note: Implement server-side code to handle file uploads in a real application.
        }
    </script>
</body>
</html>

https://github.com/user-attachments/assets/cb6f12d1-f490-451e-a898-8a9e68417fc5

