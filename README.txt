SVIMS CampusBot — Quick Setup
==============================
1. pip install -r requirements.txt
2. Copy .env.example to .env, add your Groq API key
3. Create college_docs/ folder, put SVIMS_database.pdf inside
4. python svims_server.py
5. Open http://127.0.0.1:5000

After any config change:
  curl -X POST http://127.0.0.1:5000/api/reload-config

First run builds FAISS index (2-3 min). Subsequent runs are fast.
