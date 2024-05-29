# gpt-assistants-api-ui

* 💬 OpenAI Assistants API chat UI
* 🛠️ It works easily by setting the ASSISTANT ID
* 📁 Supports file upload and file download
* 🏃 Supports Streaming API
* ~🪟 Support to Azure OpenAI~
  * ※ Cannot be used until Azure OpenAI Service supports Streaming API

<img width="1459" alt="スクリーンショット 2023-11-20 2 23 51" src="https://github.com/ryo-ma/gpt-assistants-api-ui/assets/6661165/5c288d51-196a-4919-bc4d-dc508146f58a">

## 🌟 Quick Start

1. 👤 Create an assistant on the OpenAI site & Get assistant ID (https://platform.openai.com/assistants)
2. 🔑 Get the API key from OpenAI (https://platform.openai.com/api-keys)
3. ⬇️ Clone the repository

    ```bash
    $ git clone https://github.com/ryo-ma/gpt-assistants-api-ui.git
    ```

4. 📦 Install dependencies

    ```bash
    $ poetry install
    ```

5. 🔑 Set environment variables

    ```bash
    OPENAI_API_KEY="sk-xxx"
    ASSISTANT_ID="asst_xxx"

    ASSISTANT_TITLE="Assistants API UI"
    ENABLED_FILE_UPLOAD_MESSAGE="Upload a file" # Leave empty to disable
    ```
    If you use azure instead, set `AZURE_OPENAI_ENDPOINT` and `AZURE_OPENAI_KEY`

6. 🏃‍️ Run the app

    ```bash
    $ poetry shell
    $ streamlit run app.py
    ```

## 🐳 Run the app using Docker

1. 👤 Create an assistant on the OpenAI site & Get assistant ID (https://platform.openai.com/assistants)
2. 🔑 Get the API key from OpenAI (https://platform.openai.com/api-keys)
3. ⬇️ Clone the repository

    ```bash
    $ git clone https://github.com/ryo-ma/gpt-assistants-api-ui.git
    ```
    
4. 🔑 Set environment variables

    Create a .env file.
   
    ```bash
    OPENAI_API_KEY="sk-xxx"
    ASSISTANT_ID="asst_xxx"

    ASSISTANT_TITLE="Assistants API UI"
    ENABLED_FILE_UPLOAD_MESSAGE="Upload a file" # Leave empty to disable
    ```
    If you use Azure instead, set `AZURE_OPENAI_ENDPOINT` and `AZURE_OPENAI_KEY`
    
6. 💽 Build image

    ```bash
    $ docker compose build
    ```

7. 🏃‍️ Run the app

    ```bash
    $ docker compose up
    ```
Access to [http://localhost:8501](http://localhost:8501).

