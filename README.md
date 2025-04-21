# Langchain Course Challenge

## Assignment 1: Chaining Haiku Prompts in LangChain

- **Scope**: 2.0 ~ 3.5
- **Objective**: This challenge is to familiarize ourselves with the Jupyter Notebooks, LangChain Expression Language and the submission process.

### 📌 Task

- [x] Create a Github Repository
  > → https://github.com/kangdongil/langchain-gpt-challenge
- [x] Create a Python environment.
  > → Used `pyenv` to set Python 3.11.6 and created a virtual environment.
- [x] Install dependencies.
- [x] Create a Jupyter Notebook.
  > → `notebook.ipynb`
- [x] Setup your OpenAI Keys.
  > → Stored securely in `.env`, excluded via `.gitignore`.
- [x] Make two chains and chain them together using LCEL.
  > → Combined chains using the `|` operator.
- [x] Push the code to Github

### 🔗 LCEL Chains Requirements

- [x] Make a chain that is specialized in writing Haikus about programming languages and another one that is specialized in explaining Haikus.
  > → Implemented `haiku_writer_prompt` and `haiku_curator_prompt`  
  > → Used triple quotes (`"""`) for multiline `SystemMessage` content
- [x] Chain the two chains together using LCEL.
- [x] The final chain should receive the name of a programming language and it should reply with the Haiku and its explanation.

> ```python
> final_chain = {"haiku": haiku_writer_chain} | haiku_curator_chain
> ```

- [x] Use "gpt-3.5-turbo" as the model and ChatPromptTemplate for your prompts.

> ```python
> chat = ChatOpenAI(
>     model="gpt-3.5-turbo",
>     ...
> )
> ```
