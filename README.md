
# 🔎 LangChain - Chat with Search

This repository contains a Streamlit app that allows users to interact with a chatbot capable of searching the web using LangChain. The app integrates with APIs like Arxiv, Wikipedia, and DuckDuckGo to retrieve information and provide insightful responses.

## 🚀 Features

- **Search the Web**: Retrieve results from DuckDuckGo, Wikipedia, and Arxiv.
- **Interactive Chat Interface**: Powered by Streamlit's `st.chat_message` feature.
- **Streamlit Callback Handler**: Displays agent thoughts and actions in real-time.
- **Customizable API Key Input**: Securely input your Groq API Key via the Streamlit sidebar.

## 🛠️ Tech Stack

- **Streamlit**: For building the web interface.
- **LangChain**: For managing agents and tools.
- **Arxiv, Wikipedia, DuckDuckGo APIs**: For fetching external data.

## 📦 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/MDalamin5/MultiAgent-Search-Bot-LLM.git
   cd MultiAgent-Search-Bot-LLm
   ```

2. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Create a `.env` file and add your API keys:
   ```
   GROQ_API_KEY=your_groq_api_key
   ```

4. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```

## 🖥️ How to Use

1. Launch the app using the `streamlit run app.py` command.
2. Enter your Groq API key in the sidebar.
3. Type your query in the chat input (e.g., *What is machine learning?*).
4. View the chatbot's response and actions.

## 📄 Code Explanation

### Tools Integration

- **Arxiv**: Fetches the top search result with a character limit for the content.
- **Wikipedia**: Retrieves the top search result with a character limit for the content.
- **DuckDuckGo**: General-purpose web search.

### Agent Initialization

The LangChain agent is initialized with the following:
- `tools`: Search tools from Arxiv, Wikipedia, and DuckDuckGo.
- `ChatGroq`: LLM powered by Groq API.
- `AgentType.ZERO_SHOT_REACT_DESCRIPTION`: Handles dynamic queries with zero-shot reasoning.

### Streamlit Features

- **Sidebar**: Allows users to input their Groq API key.
- **Chat Interface**: Facilitates communication with the chatbot.
- **Callback Handler**: Displays the agent's thoughts and actions dynamically.

## 🌟 Example Usage

1. **Input**: What is machine learning?
2. **Agent Response**:
   - Searches Arxiv for relevant papers.
   - Fetches summaries from Wikipedia.
   - Provides a combined response from all tools.

## 🤝 Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue.

## 📜 License

This project is licensed under the [GPL-3.0 license](LICENSE).

## 🙌 Acknowledgments

- [LangChain](https://langchain.com)
- [Streamlit](https://streamlit.io)
- [Arxiv API](https://arxiv.org)
- [Wikipedia API](https://www.mediawiki.org/wiki/API:Main_page)
- [DuckDuckGo API](https://duckduckgo.com)

---

Feel free to fork and star this repository! 🌟
