**CodeShift: C++ ↔ Pseudocode Translator**
**Overview**
CodeShift is an AI-powered tool that translates between C++ and pseudocode using a transformer model. Built with PyTorch and deployed via Streamlit, it’s ideal for developers and educators.
**Features**
Bidirectional translation (C++ → Pseudocode, Pseudocode → C++).

Interactive web interface with a coding-themed design.
Efficient transformer-based architecture.
**Prerequisites**
Python 3.11+
PyTorch, Streamlit, torchtext, numpy
**Installation**
**Clone the repo:**
git clone https://github.com/your-username/code-translator.git
cd code-translator
**Set up a virtual environment:**
python -m venv venv
Windows: venv\Scripts\activate
Mac/Linux: source venv/bin/activate
**Install dependencies:**
pip install -r requirements.txt
**Usage**
**Run locally:**
streamlit run app.py
Enter C++ or pseudocode in the web interface to translate.

**Deployment on Streamlit Community Cloud**
Push code to GitHub.
Go to share.streamlit.io, sign in with GitHub, and deploy using:
Repository: your-username/code-translator
Branch: main
Main file: app.py
**Known Issues**
Translations may repeat tokens (e.g., = 10 = 10...). Fix by retraining the model or adjusting translate in app.py
**Contact**
For questions, contact [Syed Burhan ud din ] at [hafizburhan0684@gmail.com].
