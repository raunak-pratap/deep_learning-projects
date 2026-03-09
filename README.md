<h1>MNIST Digit Classification: CNN vs. RNN (LSTM)</h1>

<p>
        This project explores two different approaches to solving the classic MNIST handwritten digit classification problem using <strong>PyTorch</strong>. 
        The goal was to compare a spatially-aware model (<strong>CNN</strong>) against a sequence-aware model (<strong>RNN/LSTM</strong>) to see how they perform on the same dataset.
    </p>

<hr>

 <h2>📌 Project Overview</h2>
    <ul>
        <li><strong>Dual Architectures:</strong> Implemented a 3-layer Convolutional Neural Network and a 2-layer LSTM-based Recurrent Neural Network.</li>
        <li><strong>Data Pipeline:</strong> Used <code>torchvision</code> for normalization and data augmentation.</li>
        <li><strong>GPU Acceleration:</strong> Utilized <strong>CUDA</strong> for efficient training on a T4 GPU.</li>
        <li><strong>Performance Tracking:</strong> Monitored training loss across 10 epochs for both models.</li>
    </ul>

 <h2>📊 Results Comparison</h2>
    <table border="1">
        <thead>
            <tr>
                <th>Model</th>
                <th>Test Accuracy</th>
                <th>Final Training Loss</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td><strong>CNN</strong></td>
                <td>98.79%</td>
                <td>0.0103</td>
            </tr>
            <tr>
                <td><strong>RNN (LSTM)</strong></td>
                <td>98.78%</td>
                <td>0.0189</td>
            </tr>
        </tbody>
    </table>

<h2>🛠️ Tech Stack</h2>
    <ul>
        <li><strong>Language:</strong> Python</li>
        <li><strong>Framework:</strong> PyTorch (<code>torch</code>, <code>nn</code>, <code>optim</code>)</li>
        <li><strong>Visualization:</strong> Matplotlib</li>
        <li><strong>Environment:</strong> Google Colab / GPU T4</li>
    </ul>

  <h2>🧠 Technical Deep Dive</h2>
    
  <h3>Convolutional Neural Network (CNN)</h3>
    <p>
        The CNN utilizes three convolutional layers with increasing filters (32, 64, 128) and MaxPool layers to extract spatial features from the 28x28 images.
    </p>

 <h3>Recurrent Neural Network (RNN/LSTM)</h3>
    <p>
        The LSTM treats each image as a sequence of 28 rows, where each row contains 28 features. 
        This approach treats image recognition as a temporal sequence problem.
    </p>

 <hr>

 <p><em>This project was developed as part of the <strong>Prime AI/ML batch</strong>  program.</em></p>

</body>
</html>
