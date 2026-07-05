<h1>FloraScan – Plant Disease Detection (VGG19 + Flask)</h1>

<p>
FloraScan is an AI-powered web application that detects plant diseases from leaf images using a VGG19 deep learning model. 
It provides predicted disease name, symptoms, remedies, and generates a downloadable PDF report that includes the uploaded image.
</p>

<p>
This project is part of a final-year BCA submission and demonstrates skills in machine learning, deep learning, Flask backend development, and report generation.
</p>

<hr>

<h2>Features</h2>
<ul>
  <li>AI-based plant disease prediction (38 classes)</li>
  <li>VGG19 deep learning model</li>
  <li>PDF report generation</li>
  <li>Uploaded image embedded inside the report</li>
  <li>Symptoms and remedies loaded from disease_info.py</li>
  <li>Flask backend with clean routing</li>
  <li>Responsive and simple user interface</li>
  <li>Auto-saved predictions in timestamped folders</li>
</ul>

<hr>

<h2>Dataset</h2>
<p>
The model is trained using the publicly available Kaggle dataset:
</p>
<p>
<b>New Plant Diseases Dataset:</b> 
<a href="https://www.kaggle.com/datasets/vipoooool/new-plant-diseases-dataset">https://www.kaggle.com/datasets/vipoooool/new-plant-diseases-dataset</a>
</p>

<p>
Note: The dataset is not included in this repository due to its large size. 
Download it manually from Kaggle and place it inside a <code>data/</code> folder if you want to retrain the model.
</p>

<hr>

<h2>Model Information</h2>
<ul>
  <li>Model: VGG19 (Transfer Learning)</li>
  <li>Input size: 256 × 256 × 3</li>
  <li>Framework: TensorFlow / Keras</li>
  <li>Classes: 38 plant diseases</li>
</ul>

<p>
The trained model file <code>florascan_modelvgg19.h5</code> is not included in the repository due to size limitations.
Use the notebook in the <code>notebooks/</code> folder to train your own model or download your pre-trained model.
</p>

<hr>

<h2>Project Structure</h2>

<pre>
FloraScan/
│
├── app.py                     # Flask backend
├── disease_info.py            # Symptoms and remedies
├── requirements.txt           # Python dependencies
├── README.md                  # Documentation
├── .gitignore                 # Ignored files
│
├── templates/                 # HTML UI pages
├── static/                    # CSS, JS, assets
│   └── results/
│       ├── images/            # Saved uploaded images (ignored)
│       └── reports/           # Generated PDF reports (ignored)
│
└── notebooks/
    └── florascan.ipynb        # Model training notebook
</pre>

<hr>

<h2>Installation and Setup</h2>

<h3>1. Create a Virtual Environment (Python 3.10 required)</h3>
<pre>py -3.10 -m venv .venv</pre>

<h3>2. Activate Environment (Windows)</h3>
<pre>.venv\Scripts\activate</pre>

<h3>3. Install Dependencies</h3>
<pre>pip install -r requirements.txt</pre>

<h3>4. Run the Application</h3>
<pre>python app.py</pre>

<p>Open in browser: http://127.0.0.1:5000/</p>

<hr>

<h2>PDF Report Output</h2>
<p>
Each generated report includes:
</p>
<ul>
  <li>Uploaded leaf image</li>
  <li>Predicted disease</li>
  <li>Symptoms</li>
  <li>Remedies</li>
  <li>Timestamp</li>
</ul>

<p>Reports are saved in:</p>
<pre>static/results/reports/</pre>

<hr>

<h2>Model Training</h2>
<p>
Training code is available in:
</p>
<pre>notebooks/florascan.ipynb</pre>

<p>
It includes:
</p>
<ul>
  <li>Data loading</li>
  <li>Data augmentation</li>
  <li>VGG19 fine-tuning</li>
  <li>Accuracy and loss graphs</li>
  <li>Confusion matrix</li>
  <li>Exporting the trained model (.h5)</li>
</ul>

<hr>

<h2>Git Ignore Information</h2>
<p>
This repository excludes:
</p>

<pre>
.venv/
data/
*.h5
static/results/images/
static/results/reports/
</pre>

<p>
This keeps the project lightweight and prevents uploading large files.
</p>

<hr>

<h2>Author</h2>
<p><b>Sarvika SJ</b><br>BCA Final Year Project<br>FloraScan – Plant Disease Diagnosis</p>

<hr>
<p>If you found this project helpful, please star the repository on GitHub.</p>
