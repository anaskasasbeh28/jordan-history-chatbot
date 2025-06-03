
# Jordanian History Chatbot 🇯🇴

This is a simple chatbot application that uses OpenAI's GPT model to simulate a **Jordanian history tutor**.  
The chatbot maintains conversation context and can be interacted with via the terminal.

---

## 📚 Features

- Chatbot with memory (remembers full conversation)
- Customizable system prompt
- Word and token counting using `tiktoken`
- Works with OpenAI's `gpt-3.5-turbo`

---

## 🛠 Requirements

- Python 3.8+
- OpenAI Python SDK
- `tiktoken` package

You can install the required libraries with:

```bash
pip install openai tiktoken
````

---

## 🚀 How to Run

1. Replace your OpenAI API Key inside the script:

```python
os.environ['OPENAI_API_KEY'] = 'your-api-key-here'
```

2. Run the script and start chatting:

```python
history_tutor = CreateBot(system_prompt='You are a Jordanian History Tutor')
history_tutor.chat()
```

To end the conversation, type: `END`

---

## 🧠 Word & Token Counter

After chatting, the script will:

* Combine all messages
* Count the number of **words**
* Count the number of **tokens** (using `cl100k_base` tokenizer)

---

## 📦 File Structure

```
chatbot_openai_token_analysis.py   # Main Python script
README.md                          # This file
```

---

## ✍️ Example Interaction

```text
User: Who was the first king of Jordan?
Bot: The first king of Jordan was King Abdullah I.

User: What year was he born?
Bot: King Abdullah I was born in 1882.
```

---

## 🧠 Future Improvements

* Web-based interface (e.g. Streamlit)
* Arabic/Jordanian dialect support
* Saving conversation logs

---

## 🧑‍💻 Author

Made with ❤️ by Anas and ChatGPT 🙌

---

## 🪪 License

This project is for educational purposes only.

---
