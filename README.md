CodeShift: C++ ↔ Pseudocode Translator
Overview
CodeShift is an AI-powered tool that translates between C++ code and pseudocode using a custom transformer model. Built with PyTorch and deployed as a web application using Streamlit, this project enables developers to convert C++ code into readable pseudocode (and vice versa) for better code understanding, documentation, or educational purposes. The model leverages a sequence-to-sequence transformer architecture trained on a dataset of C++ and pseudocode pairs, making it a valuable resource for programmers and educators alike.

Features
Bidirectional Translation: Convert C++ code to pseudocode and pseudocode back to C++.
Interactive Web Interface: A user-friendly, coding-themed UI built with Streamlit, accessible via the browser.
Efficient Transformer Model: Uses a custom Seq2SeqTransformer with positional encoding for accurate translations.
Cross-Platform: Tested and deployable on local machines or Streamlit Community Cloud.
Prerequisites
Before running or deploying CodeShift, ensure you have the following installed:

Python (3.11 or higher recommended)
PyTorch (for the transformer model)
Streamlit (for the web interface)
Other Dependencies: torchtext, numpy
Installation
Clone the Repository
bash
Wrap
Copy
git clone https://github.com/your-username/code-translator.git
cd code-translator
Set Up a Virtual Environment
Create and activate a virtual environment to manage dependencies:

bash
Wrap
Copy
python -m venv venv
Windows:
bash
Wrap
Copy
venv\Scripts\activate
Mac/Linux:
bash
Wrap
Copy
source venv/bin/activate
Install Dependencies
Install the required packages using the provided requirements.txt:

bash
Wrap
Copy
pip install -r requirements.txt
Download Model Files and Vocabulary
Ensure the following files are in your project directory:

vocabulary.json: The vocabulary file mapping tokens to indices.
cpp_to_pseudo_epoch_1.pth: The trained model checkpoint for C++ to pseudocode translation.
transformer_epoch_1.pth: The trained model checkpoint for pseudocode to C++ translation.
You can download these files from the repository or provide them manually if hosted elsewhere (e.g., Google Drive).

Usage
Running Locally
Navigate to the project directory in your terminal.
Launch the Streamlit app:
bash
Wrap
Copy
streamlit run app.py
Open your browser to the URL provided (e.g., http://localhost:8501).
Use the interface to input C++ or pseudocode, select the translation mode (C++ → Pseudocode or Pseudocode → C++), and click "Translate" to see the result.
Example Inputs
C++ Input: int a = 10;
Expected Output (Pseudocode): create integer a with value 10
Pseudocode Input: create integer a with value 10
