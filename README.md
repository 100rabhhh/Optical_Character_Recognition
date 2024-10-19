<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
    <h1>📜 Optical Character Recognition (OCR) Project</h1>
    <p>🚀 <strong>Welcome to the Optical Character Recognition (OCR) Project!</strong> This project leverages <strong>EasyOCR</strong> and <strong>OpenCV</strong> to extract and recognize text from images, making it easy to convert scanned documents, signs, or handwritten text into machine-readable formats. With just a few lines of code, you can easily implement OCR in your own projects!</p>
    <h2>✨ Features</h2>
    <ul>
        <li>📸 <strong>Image Input</strong>: Easily load any image for OCR processing.</li>
        <li>🔍 <strong>Text Detection</strong>: Recognizes text with bounding boxes using EasyOCR.</li>
        <li>🎨 <strong>Result Visualization</strong>: Visualizes detected text with bounding boxes using OpenCV and Matplotlib.</li>
        <li>📝 <strong>Handles Multiple Lines</strong>: Detects and processes multiple lines of text seamlessly.</li>
    </ul>
    <h2>🔧 Installation</h2>
    <pre><code>pip3 install torch torchvision torchaudio
pip install easyocr opencv-python matplotlib</code></pre>
    <h2>🚀 How to Use</h2>
    <ol>
        <li><strong>Load an Image</strong>: Replace the image path with the one you want to process in the notebook.
            <pre><code>IMAGE_PATH = 'your_image_here.png'</code></pre>
        </li>
        <li><strong>Perform OCR</strong>:
            <pre><code>reader = easyocr.Reader(['en'])
result = reader.readtext(IMAGE_PATH)</code></pre>
        </li>
        <li><strong>Visualize the Results</strong>:
            <pre><code># Visualize detected text with bounding boxes
for detection in result:
    print(detection)</code></pre>
        </li>
    </ol>
    <h2>📖 Libraries Used</h2>
    <ul>
        <li><strong>EasyOCR</strong>: A Python library for Optical Character Recognition, helping to read and extract text from images.</li>
        <li><strong>OpenCV</strong>: A computer vision library used for loading images and drawing bounding boxes around detected text.</li>
        <li><strong>Matplotlib</strong>: A visualization library used to display the image with bounding boxes.</li>
    </ul>
    <h2>🚀 How It Works</h2>
    <ol>
        <li><strong>Loading the Image</strong>: The image is loaded using OpenCV's <code>cv2.imread()</code>.</li>
        <li><strong>OCR (Text Detection)</strong>: The image is passed through <strong>EasyOCR</strong>, extracting text and bounding box coordinates.</li>
        <li><strong>Drawing Bounding Boxes</strong>: Using OpenCV, bounding boxes are drawn around the detected text.</li>
        <li><strong>Text Overlay</strong>: The recognized text is overlayed on top of the image using OpenCV.</li>
        <li><strong>Displaying the Result</strong>: The final image is displayed using Matplotlib with the text detected and highlighted.</li>
    </ol>
    <h2>📊 Example Output</h2>
    <p>The detected text is <strong>"HEAD PROTECTION MUST BE WORN ON THIS SITE"</strong>, with bounding boxes drawn around the text.</p>
    <h2>👨‍💻 Technologies Used</h2>
    <ul>
        <li><strong>Python</strong> 🐍</li>
        <li><strong>EasyOCR</strong> 📖</li>
        <li><strong>OpenCV</strong> 📷</li>
        <li><strong>Matplotlib</strong> 📊</li>
    </ul>
    <h2>💡 Future Enhancements</h2>
    <ul>
        <li>Extend OCR to work with non-English languages.</li>
        <li>Implement batch processing for multiple images.</li>
    </ul>
    <h2>🔚 Conclusion</h2>
    <p>This project showcases how Optical Character Recognition (OCR) can be effectively implemented using Python libraries such as EasyOCR and OpenCV. It demonstrates the ability to accurately detect and extract text from images, making it a powerful tool for text recognition tasks. The project's flexible and simple implementation allows for future enhancements, such as adding more languages and improving batch processing capabilities.</p>
</body>
</html>
