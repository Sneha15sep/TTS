Clarity TTS Fine-Tuning Project

Table of Contents
Prerequisites
Installation
Dataset Preparation
Running the Fine-Tuning
Evaluation
Fast Inference Optimization (Bonus Task)
Conclusion
Prerequisites


#Before running the code, ensure you have the following:

Python 3.7 or higher
PyTorch 1.10 or higher
Coqui TTS library
Other necessary libraries

#Installation
Clone the repository:
git clone <repository-url>
cd <repository-folder>

Install the required packages:
pip install -r requirements.txt

#Dataset Preparation
Prepare your dataset by following these steps:
For the English technical vocabulary dataset, ensure it includes terms like 'API', 'CUDA', etc.
For the regional language, download the Common Voice dataset and preprocess it.
Update the dataset path in the configuration file (config.json).

#Running the Fine-Tuning
Navigate to the training directory:
cd <training-directory>

Start the fine-tuning process:
python train.py --config config.json

Monitor the training progress via logs saved in the specified directory.
#Evaluation
After training, evaluate the model using:
python evaluate.py --model <model-path>

Check the output logs and generated audio samples for MOS scores and pronunciation accuracy.

#Fast Inference Optimization (Bonus Task)
To run inference optimization
Check the output logs and generated audio samples for MOS scores and pronunciation accuracy.
Fast Inference Optimization (Bonus Task)
To run inference optimization:
python optimize.py --model <model-path>

Evaluate the optimized model's performance against the original.
Copy code
python optimize.py --model <model-path>
Evaluate the optimized model's performance against the original.
