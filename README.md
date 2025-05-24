# 🧾 PDF Chatbot with NVIDIA NIM & LLaMA3-70B
Ask Questions from Any Document — Instantly.

This application allows users to chat with any kind of PDF — reports, manuals, contracts, legal papers, books, or datasets — using NVIDIA NIM powered by LLaMA3-70B. It converts your uploaded documents into embeddings, enabling semantic search and context-aware responses using LangChain’s RAG framework.

## 📌 Features
* 🧠 Chat with your PDF documents using natural language — not just academic papers
* 🏎️ Uses NVIDIA NIM + LLaMA3-70B-Instruct for ultra-fast LLM inference
* 🔍 Multi-PDF ingestion and chunking with vector search via FAISS
* 🔗 Built with LangChain's RAG architecture and Streamlit frontend
* 📁 Upload any collection of PDFs into a local folder and interact immediately

## 🧠 Technologies Used
* NVIDIA NIM – Model Inference for LLaMA3 via NVIDIA cloud
* LangChain – Document chains, embedding pipelines, retrievers
* Streamlit – Interactive web interface
* FAISS – High-performance vector search
* NVIDIAEmbeddings – For creating semantic vectors
* LLaMA3-70B-Instruct – Model used for answering user queries

## 🗂 Project Structure
```
├── finalapp.py             # Main Streamlit app logic
├── app.py                  # Direct model API test (NVIDIA NIM usage example)
├── us_census/              # Folder where PDFs are placed
├── requirements.txt        # Python dependencies
└── .env                    # Contains your NVIDIA_API_KEY (excluded from repo)
```

1. Clone the Repository
```
git clone https://github.com/bhaskar2311/PDF-Chatbot-NVDIA-NIM-Llama3-70B
cd PDF-Chatbot-NVDIA-NIM-Llama3-70B
```
2. Create a Virtual Environment (optional but recommended)
```
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```
3. Install Dependencies
```
pip install -r requirements.txt
```
4. Setup Environment Variables
  * Create a .env file in the root directory and add your API keys like this:
```
# .env
NVIDIA_API_KEY=your_nvidia_api_key_here
```
🚨 Warning: Never commit .env files to public repositories.



## 📁 How to Use
* Place your PDFs inside the us_census/ folder (or rename it as needed).
* Run the app:
```
streamlit run finalapp.py
```
* Click the "Documents Embedding" button.
* Ask any question related to your documents — e.g.:
  - "What is the summary of this document?"
  - "Which state had the highest uninsured rate in 2022?"
  - "List all data protection policies mentioned."

* View instant answers and document similarity context side-by-side.

## 📝 Points to keep in mind
* ❗ This chatbot works on any PDFs, not just research papers.
* You can ingest multiple documents — up to 30 PDFs (customizable in code).
* The app uses RecursiveCharacterTextSplitter for smart chunking.
* Designed to showcase NVIDIA’s inference power via NIM cloud APIs.

## 📸 Screenshot
![Output](https://github.com/user-attachments/assets/8b86b836-b6f1-472b-8133-fbca7ccc670f)

## 📝 Notes
This project was fully developed by me. The README was written based on my knowledge and experience, with support from generative AI tools to refine its structure and presentation.

## 📄 License
This project is open source and available under the MIT License.

## 🙋‍♂️ Author
Made with ❤️ by Bhaskar Shivaji Kumbhar

