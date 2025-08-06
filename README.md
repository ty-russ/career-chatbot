# Portfolio Website AI Chat Bot

A Gradio‑powered chat interface that represents **Tirus Kimani Wagacha** authentically on his personal website. This bot:

- Uses the OpenAI API to answer questions in the voice of Tirus, based on his LinkedIn profile and summary.
- Logs visitor‑provided contact details (email, name, notes) via Pushover notifications.
- Records any unanswered questions for future review.

---

## Summary

A lightweight AI chat assistant embedded right in your portfolio – powered by Gradio and OpenAI, this bot interacts as you, captures visitor leads via Pushover notifications, and logs any unanswered questions for continuous improvement.

## 📂 Repository Structure

```
├── files/
│   ├── linkedin.pdf       # LinkedIn profile PDF
│   └── summary.txt        # Plain‑text summary of professional background
├── app.py                 # Main application script
├── requirements.txt       # Python dependencies
└── README.md              
```

---

## 🚀 Features

- **Branded AI Persona**: Leverages a rich system prompt (LinkedIn + summary) so the bot speaks as Tirus.
- **Gradio Chat UI**: Easy‑to‑embed chat widget for any website.
- **Contact Capture**: `record_user_details` tool logs visitor emails/names/notes via Pushover.
- **Unknown Question Logging**: `record_unknown_question` captures queries the bot can’t answer.
- **Extensible**: Add more tools or adjust the system prompt to evolve the persona.

---

## ⚙️ Installation

1. **Clone the repo**

   ```bash
   git clone https://github.com/yourusername/website-ai-chat.git
   cd website-ai-chat
   ```

2. **Create a virtual environment & activate**

   ```bash
   python3 -m venv venv
   source venv/bin/activate    # macOS/Linux
   venv\Scripts\activate     # Windows
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

---

## 🔧 Configuration

Create a `.env` file in the project root with the following keys:

```env
OPENAI_API_KEY=sk-...
PUSHOVER_TOKEN=your_pushover_app_token
PUSHOVER_USER=your_pushover_user_key
```

- `OPENAI_API_KEY`: API key for OpenAI access.
- `PUSHOVER_TOKEN` & `PUSHOVER_USER`: Credentials for sending notifications via Pushover.

---

## ▶️ Running Locally

```bash
python app.py
```

By default, this launches a Gradio interface at `http://127.0.0.1:7860`.

---

## 🛠️ Contributing

1. Fork this repository.
2. Create a feature branch: `git checkout -b feature-name`.
3. Commit your changes: `git commit -m "Add some feature"`.
4. Push to the branch: `git push origin feature-name`.
5. Open a Pull Request.

---

## 📄 License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.


