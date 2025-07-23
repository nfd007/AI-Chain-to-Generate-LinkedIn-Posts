**AI Chain to Generate LinkedIn Posts**

**Project Overview**
This project is a LangChain-based AI application that generates professional LinkedIn posts based on user-provided topics and languages (English, Spanish, French) using OpenAI GPT models and prompt engineering (few-shot). The goal is to automate engaging LinkedIn post creation for a variety of themes.

**Features**

- Input: Topic and language (English, Spanish, French)
- Output: Professional LinkedIn post
- LLM: OpenAI GPT-3.5/4 (any available chat model)
- Prompt engineering: Few-shot learning for style consistency
- Framework: LangChain (with ChatOpenAI)
- Colab ready: Easy to run in Google Colab


**Architecture Diagram**

<img width="652" height="306" alt="Pasted image" src="https://github.com/user-attachments/assets/0c8f1692-94f6-4f25-b4ec-cfd865aaf706" />






**Workflow Diagram**

<img width="284" height="680" alt="Pasted image (2)" src="https://github.com/user-attachments/assets/377bf765-0984-45c6-aec6-da49bb636c98" />


**Workflow Steps**

1. User inputs topic and language.
2. Prompt template is constructed with few-shot examples.
3. LangChain LLMChain combines prompt and model.
4. OpenAI GPT model generates the LinkedIn post.
5. Output is shown to the user.






**How to Run**

1. Open the provided Google Colab notebook: AI_Chain_to_Generate_LinkedIn_Posts.ipynb
2. Install required libraries:
    !pip install --upgrade langchain langchain-community openai
    !pip install -qU langchain-openai
3. Set your OpenAI API key:
    import os
    os.environ["OPENAI_API_KEY"] = "sk-..."  # Replace with your key
4. Paste the code below to define your prompt, examples, and chain (see code section).
5. Generate posts for your topics and languages (see code section).


**Customization**

- To add more languages: Add more few-shot examples in the examples list.
- Change style/tone: Edit the prefix or the sample posts for a different platform or style.


**References**

- LangChain Documentation: https://python.langchain.com/
- OpenAI Documentation: https://platform.openai.com/docs/



**Contact**

For issues or feedback, please open an issue on GitHub or contact the author.
