🌿 Harnessing Deep Learning for Precise Estimation of Indian Medicinal Leaves Characteristics




📌 Overview
This project integrates Deep Learning (VGG16) and Machine Learning (Random Forest) to identify and analyze Indian medicinal plant leaves with high precision.
Using image-based analysis, the system predicts:

Plant species name

Medicinal properties

Geographic origin

Curative uses

It is designed to support researchers, botanists, and Ayurveda practitioners in quick, scalable, and accurate medicinal plant identification.

🎯 Key Features
✅ Dual-Model Approach:

VGG16 — Deep CNN for automated feature extraction.

Random Forest — High-accuracy traditional classifier.

✅ Majority Voting — Combines both models for final prediction.

✅ Medicinal Knowledge Base — Displays uses, benefits, and origin.

✅ Streamlit Web App — Upload an image → Get instant classification.

🗂 Dataset
Source: Combination of public datasets & custom images of Indian medicinal leaves.

Format: JPEG & PNG images.

Preprocessing:

Resize to 224×224 for VGG16.

Normalize pixel values.

Apply augmentation (rotation, flip, zoom).

🛠 Tech Stack
Language: Python

Deep Learning: TensorFlow / Keras (VGG16)

Machine Learning: Scikit-learn (Random Forest)

Image Processing: OpenCV, PIL

Web Interface: Streamlit

Data Handling: NumPy, Pandas

Visualization: Matplotlib, Seaborn

⚙️ Workflow
mermaid
Copy
Edit
graph TD
A[Image Upload] --> B[Preprocessing: Resize & Normalize]
B --> C[VGG16 Feature Extraction]
C --> D1[Random Forest Classification]
C --> D2[VGG16 Classification]
D1 --> E[Majority Voting]
D2 --> E[Majority Voting]
E --> F[Medicinal Properties + Output Display]
📊 Results
Model	Accuracy
Random Forest	92%
VGG16	81%
Majority Voting	Higher combined accuracy

📸 Screenshots
Home Page

Dataset Input

User Input (Neem Leaf)

Prediction Example

VGG16 Training & Validation Accuracy

Random Forest Performance

Confusion Matrix

🚀 Installation & Usage
bash
Copy
Edit
# Clone the repository
git clone https://github.com/yourusername/Harnessing-Deep-Learning-For-Precise-Estimation-Of-Indian-Medicinal-Leaves-Characteristics.git
cd Harnessing-Deep-Learning-For-Precise-Estimation-Of-Indian-Medicinal-Leaves-Characteristics

# Install dependencies
pip install -r requirements.txt

# Run the app
streamlit run app.py
📌 Future Enhancements
Expand dataset to include rare species.

Add real-time camera classification.

Multilingual & offline mode.

GPS-based plant location mapping.

Mobile application version.

👨‍💻 Author
Nishanth B G
B.Tech in Computer Science & Engineering | Alliance University
Passionate about AI, Deep Learning, and Healthcare Technology
