<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>I Love My Girlfriend</title>
    <style>
        body {
            background-color: #f0f0f0; /* Fallback background color */
            background-image: url("heart_background.jpg"); /* Replace with your heart background image */
            background-size: cover; /* Cover the entire background */
            background-repeat: no-repeat; /* Prevent image from repeating */
            font-family: sans-serif;
            color: #333; /* Dark text for better contrast */
            margin: 0; /* Remove default margins */
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center; /* Center content horizontally */
            min-height: 100vh; /* Ensure full viewport height */
        }

        .container {
            background-color: rgba(255, 255, 255, 0.8); /* Semi-transparent white background for content */
            padding: 20px;
            border-radius: 10px;
            margin-top: 20px; /* Space from the top */
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); /* Subtle shadow */
            max-width: 800px; /* Limit container width */
        }

        h1 {
            color: #e91e63; /* Pink heading */
            text-align: center;
        }

        p {
            text-align: center;
            line-height: 1.6;
        }

        .upload-section {
            margin-top: 20px;
            text-align: center; /* Center upload elements */
        }

        input[type="file"] {
            margin-bottom: 10px;
        }

        /* Responsive adjustments */
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
        <p>This page is dedicated to the most amazing person in my life. She's kind, beautiful, and makes every day an adventure. I'm so lucky to have her, and I wanted to create a special place to share some memories.</p>
        <div class="upload-section">
            <h2>Upload Memories</h2>
            <input type="file" id="imageUpload" name="imageUpload" accept="image/*"> <br>
            <input type="file" id="videoUpload" name="videoUpload" accept="video/*">
            <button onclick="uploadFiles()">Upload</button> <br><br>
            <div id="fileStatus"></div> <br><br>
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

            fileStatus.textContent = "Uploading..."; // Initial upload message

            // In a real application, you would send these files to a server.
            // This example uses a simulated upload with setTimeout:
            setTimeout(() => {
                fileStatus.textContent = "Upload Complete (Simulated)"; // Update after "upload"
                imageUpload.value = ''; // Clear input after "upload"
                videoUpload.value = ''; // Clear input after "upload"
            }, 2000); // Simulate 2-second upload time

            // *** IMPORTANT ***
            // You'll need server-side code (e.g., Python, Node.js, PHP) to 
            // actually handle file uploads. This client-side code only 
            // selects the files. Look into using fetch or XMLHttpRequest
            // to send the files to your server.
        }
    </script>
</body>
</html>
