# 🧠 AI-Powered Code Reviewer

A lightweight full-stack application built with the MERN stack that allows developers to input code and receive real-time AI-generated reviews, error detection, and actionable improvement suggestions — powered by Google Gemini's latest LLM.


## 📌 Features

- ✨ **Instant Code Reviews**: Paste your code and get AI-generated suggestions in real time.
- 🧠 **LLM-Powered Analysis**: Uses **Google Gemini 2.0 Flash** for code review with a developer-focused system prompt.
- 🎨 **Syntax Highlighting**: Implemented with `react-simple-code-editor`, `PrismJS`, and `highlight.js`.
- 💬 **Markdown-Formatted Feedback**: Gemini responses are rendered using `react-markdown` with syntax-aware highlighting.
- ⚡ **Clean, Minimal UI**: Focused interface with just two panes – input and review.


## 🖼️ UI Screenshots

![image](https://github.com/user-attachments/assets/a6dcf292-9079-4e44-b270-8f07096fbd10)


### 🧾 Code Editor (User Input)

  ![image](https://github.com/user-attachments/assets/5384aa20-b3c1-407f-8151-1be7b90cd309)

*User pastes or types code using a syntax-highlighted editor.*

### 🤖 AI Review Output

![image](https://github.com/user-attachments/assets/6a15b34c-b443-4ba7-b1f1-4cd1836e028d)
  
*Google Gemini API returns markdown-formatted code review suggestions.*


## 🛠️ Tech Stack

**Frontend:**
- React.js
- Axios
- `react-simple-code-editor`
- PrismJS
- Highlight.js
- `react-markdown`
- `rehype-highlight`

**Backend:**
- Node.js
- Express.js
- Google Generative AI SDK (Gemini 2.0 Flash)

---

## 🔍 How It Works

1. User pastes code into the editor pane.
2. On clicking **Review**, the code is sent to the backend via a POST request.
3. The backend passes the code along with a detailed system prompt to the **Gemini API**.
4. Gemini analyzes the code and returns feedback including:
   - 🔍 Issues found
   - ✅ Recommended fixes
   - 💡 Suggested improvements
5. The frontend renders the markdown response with syntax highlighting.
