```markdown
# Digital-Persona-AI

Digital Persona / AI that acts like you using information from your LinkedIn profile.

This project creates a chatbot that answers questions as if it were the person whose professional information is provided. The bot uses a LinkedIn PDF and a summary file to represent the person's career, background, and skills.

---

# LinkedPersona AI 🤖

An AI chatbot that acts like a professional digital persona using information from a LinkedIn profile.

The system loads:

- A LinkedIn profile exported as a **PDF**
- A **summary.txt** file describing the person

This information is inserted into the **system prompt**, allowing the model to answer questions as if it were that person.

---

# 🚀 Project Overview

The chatbot represents a professional persona and answers questions about:

- Career
- Skills
- Experience
- Background

Instead of reading a resume or LinkedIn page, users can simply **chat with the persona**.

Example questions:

- "What projects have you worked on?"
- "What are your key skills?"
- "Tell me about your experience."
- "What companies have you worked at?"

---

# 🧠 How It Works

1. LinkedIn profile is loaded from a **PDF file**
2. Additional information is loaded from **summary.txt**
3. Both are inserted into a **system prompt**
4. The chatbot sends messages to an **LLM via Ollama**
5. The model answers as the person described in the data

The chatbot can also trigger tools when needed.

---

# 🛠 Tools

Two tools are available to the model:

### record_user_details
Records when a user provides contact information.

Example use:
- name
- email
- notes

A **Pushover notification** is sent when this happens.

---

### record_unknown_question
If the model cannot answer a question, it records it.

This helps track questions that the bot could not handle.

A **Pushover notification** is also sent.

---

# ⚙️ Tech Stack

| Component | Technology |
|-----------|------------|
| Language | Python |
| LLM | Ollama (Qwen model) |
| UI | Gradio |
| PDF Processing | PyPDF |
| Notifications | Pushover API |

---

# 📂 Data Used

The chatbot loads two files:

```

me/linkedin.pdf
me/summary.txt

```

These files contain the professional information used to build the persona.

---

# 💬 Example Conversation

**User**

```

What is your background?

```

**Bot**

```

I have worked on several projects and have experience in AI, machine learning, and software development.

```

---

# ▶️ Running the Project

Install dependencies:

```

pip install -r requirements.txt

```

Run the chatbot:

```

python app.py

```

The Gradio interface will start and allow users to chat with the persona.

---

# 🧩 Future Improvements

- Automatic LinkedIn data extraction
- Support for multiple personas
- Better conversation memory
- Web deployment
- Improved persona customization
```

---

Agar chaho to main **2 aur cheeze bhi improve kar sakta hoon** jo GitHub repo ko aur professional bana degi:

* **repo folder structure**
* **requirements.txt (correct dependencies)**

Ye dono usually professors aur recruiters dekhte hain.
