<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
    <h1>🎨 Neural Style Transfer using TensorFlow Hub (Single & Multiple Styles)</h1>
    <p>This repository contains Google Colab notebooks demonstrating how to apply artistic style transfer to images using TensorFlow Hub. It supports both single and multiple style image transfers on a given content image, helping users explore and understand deep learning-based visual creativity.</p>

  <h2>📋 Table of Contents</h2>
    <ul>
        <li><a href="#about">🖼️ About the Project</a></li>
        <li><a href="#structure">📂 Project Structure</a></li>
        <li><a href="#requirements">🔧 Requirements</a></li>
        <li><a href="#usage">▶️ How to Run</a></li>
        <li><a href="#output">💾 Output</a></li>
        <li><a href="#references">🔗 References</a></li>
        <li><a href="#author">🧑‍💻 Author</a></li>
    </ul>

   <h2 id="about">🖼️ About the Project</h2>
    <p>This project showcases how to apply style transfer using the <strong>Arbitrary Image Stylization v1-256</strong> model from TensorFlow Hub.</p>
    <ul>
        <li><strong>Single Style Transfer:</strong> Apply one style image to a content image.</li>
        <li><strong>Multiple Style Transfer:</strong> Apply multiple style images to a single content image automatically.</li>
    </ul>

   <h2 id="structure">📂 Project Structure</h2>
    <pre>
📁 neural_style_transfer/
│
├── single_style_transfer.ipynb       # Colab notebook for single style transfer
├── multiple_style_transfer.ipynb     # Colab notebook for applying multiple styles
├── README.html                       # This documentation file
    </pre>

   <h2 id="requirements">🔧 Requirements</h2>
    <p>The notebooks are designed for Google Colab, but if you're running locally, install the required packages:</p>
    <pre><code>pip install tensorflow tensorflow_hub matplotlib</code></pre>

  <h2 id="usage">▶️ How to Run</h2>
    <p><strong>In Google Colab:</strong></p>
    <ol>
        <li>Open either notebook from this repository in Colab.</li>
        <li>Run all cells sequentially.</li>
        <li>Upload your content and style images when prompted.</li>
    </ol>
    <p><strong>Single Style Notebook:</strong> Prompts for exactly two images.</p>
    <p><strong>Multiple Style Notebook:</strong> Prompts for one content image followed by multiple style images.</p>

  <h2 id="output">💾 Output</h2>
    <ul>
        <li>Stylized images are displayed inline and saved to the <code>stylized_outputs</code> folder.</li>
        <li>You can download the outputs using <code>files.download()</code> method.</li>
    </ul>

  <h2 id="references">🔗 References</h2>
    <ul>
        <li><a href="https://tfhub.dev/google/magenta/arbitrary-image-stylization-v1-256/2" target="_blank">TensorFlow Hub - Stylization Model</a></li>
        <li><a href="https://www.tensorflow.org/hub/tutorials/tf_hub_generative_image_stylization" target="_blank">Official TF Hub Tutorial</a></li>
        <li><a href="https://colab.research.google.com/" target="_blank">Google Colab</a></li>
    </ul>

  <h2 id="author">🧑‍💻 Author</h2>
    <p><strong>Name</strong> – <a href="https://github.com/PavanaAradhya" target="_blank">PavanaAradhya</a></p>

  <h3 id="Thank You">🌟 Thank you for checking out this project! Contributions are welcome. Happy coding and creating! 🌟</h3>

</body>
</html>
