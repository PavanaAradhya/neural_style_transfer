<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Neural Style Transfer - TensorFlow Hub (Colab)</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.7;
      max-width: 960px;
      margin: auto;
      padding: 2rem;
      background-color: #f9f9f9;
      color: #333;
    }
    h1, h2 {
      color: #2b5dff;
    }
    code {
      background-color: #eee;
      padding: 2px 5px;
      border-radius: 4px;
      font-family: monospace;
    }
    pre {
      background: #f4f4f4;
      padding: 1rem;
      overflow-x: auto;
      border-left: 4px solid #2b5dff;
    }
    .section {
      margin-top: 40px;
    }
    .note {
      background: #fffbe6;
      border-left: 4px solid #ffc107;
      padding: 1rem;
      margin: 1rem 0;
    }
  </style>
</head>
<body>

  <h1>🎨 Neural Style Transfer using TensorFlow Hub</h1>

  <p>This project demonstrates how to use <strong>TensorFlow Hub</strong> to apply artistic style transfer to images using Google Colab.</p>

  <div class="note">
    <strong>Model Used:</strong> 
    <a href="https://tfhub.dev/google/magenta/arbitrary-image-stylization-v1-256/2" target="_blank">
      Magenta Arbitrary Image Stylization v1-256
    </a>
  </div>

  <div class="section">
    <h2>🔹 1. Single Style Transfer</h2>
    <p>Use one content image and one style image to generate a stylized output.</p>

    <p><strong>Steps:</strong></p>
    <ul>
      <li>Upload content and style images</li>
      <li>Load and preprocess them</li>
      <li>Apply the pre-trained TF Hub model</li>
      <li>Visualize and optionally save the output</li>
    </ul>

    <p><strong>Colab Link:</strong> <a href="#">(Insert Your Colab URL)</a></p>
  </div>

  <div class="section">
    <h2>🔸 2. Multiple Style Transfer</h2>
    <p>Use one content image with multiple style images. The script will generate one stylized output per style image.</p>

    <p><strong>Steps:</strong></p>
    <ul>
      <li>Upload 1 content image and multiple style images</li>
      <li>Images are preprocessed safely (invalid files are skipped)</li>
      <li>Each style is applied to the content image individually</li>
      <li>All outputs are saved to <code>stylized_outputs/</code> folder</li>
    </ul>

    <p><strong>Features:</strong></p>
    <ul>
      <li>Error handling for unsupported/corrupted image files</li>
      <li>Automatic display of input/output images</li>
      <li>Results saved as JPGs</li>
    </ul>

    <p><strong>Colab Link:</strong> <a href="#">(Insert Your Colab URL)</a></p>
  </div>

  <div class="section">
    <h2>💾 Output Folder</h2>
    <p>Stylized images are saved to a folder named <code>stylized_outputs</code> in the Colab environment. You can use this snippet to download them:</p>

    <pre><code>from google.colab import files
import glob

for file in glob.glob("stylized_outputs/*.jpg"):
    files.download(file)</code></pre>
  </div>

  <div class="section">
    <h2>🧠 Model Details</h2>
    <ul>
      <li><strong>Name:</strong> Arbitrary Image Stylization v1-256</li>
      <li><strong>Source:</strong> <a href="https://tfhub.dev/google/magenta/arbitrary-image-stylization-v1-256/2" target="_blank">TensorFlow Hub</a></li>
      <li><strong>Input:</strong> 2 images (content, style)</li>
      <li><strong>Output:</strong> Stylized image</li>
    </ul>
  </div>

  <div class="section">
    <h2>📎 References</h2>
    <ul>
      <li><a href="https://www.tensorflow.org/hub/tutorials/tf_hub_generative_image_stylization" target="_blank">TensorFlow Hub Stylization Tutorial</a></li>
      <li><a href="https://colab.research.google.com" target="_blank">Google Colab</a></li>
    </ul>
  </div>

</body>
</html>
