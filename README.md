# 🚀 LLM-based Automation Agent  

Welcome to the **LLM-based Automation Agent**! This intelligent automation agent leverages natural language processing and LLM capabilities to handle a variety of tasks seamlessly.  

This project is a task automation system that uses a language model to parse and execute various tasks. The system is built using FastAPI for the API, and it supports a variety of tasks such as fetching data from APIs, handling git operations, running SQL queries, web scraping, image processing, and more.

---

## 🌟 Features  
- 🤖 **Task Parsing**: Powered by GPT-4o-Mini for accurate task interpretation.  
- 🔒 **Secure File Operations**: Ensures safe and secure handling of sensitive files.  
- ⚡ **Multi-Task Support**: Efficiently handles multiple task types.  
- 🌐 **API-Based Execution**: Executes tasks using powerful API integrations.  
- Task parsing using a language model
- Task execution with various handlers
- API endpoints for running tasks and reading files
- CORS support for cross-origin requests
- Docker support for containerization

---

## 📋 Prerequisites  
Make sure you have the following installed:  
- **Docker**: For containerization and deployment.  
- **AI Proxy Token**: Required for accessing LLM functionalities.  
- Python 3.9
- Node.js and npm (for Prettier)

---

## ⚙️ Installation & Run  

### 1. Clone the Repository  
```sh
git clone https://github.com/amangour01/llm-agent.git
```
``` 
cd llm-agent
```

### 2. Install Dependencies  
```
pip install -r requirements.txt  
```

### 3. Setup Environment Variables  
### Create a .env file in the project root  
```
echo "AIPROXY_TOKEN=your_token_here" > .env  
```

### 4. Run Locally  
```
python run.py  
```

### 5. Using Docker  
### Build the image  
```
docker build -t llm-agent .  
```

### Run the container  
```
docker run --env-file .env -p 8000:8000 llm-agent  
```

## Installation

1. Clone the repository:

    ```sh
    git clone https://github.com/yourusername/llm-agent.git
    cd my-llm
    ```

2. Create a virtual environment and activate it:

    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required Python packages:

    ```sh
    pip install -r requirements.txt
    ```

4. Install Prettier globally using npm:

    ```sh
    npm install -g prettier@3.4.2
    ```

5. Create a `.env` file in the root directory and add your API proxy token:

    ```properties
    AIPROXY_TOKEN="your_api_proxy_token"
    ```

## Running the Application

1. Start the FastAPI server:

    ```sh
    python run.py
    ```

2. The API will be available at `http://0.0.0.0:8000`.

## Using Docker

1. Build the Docker image:

    ```sh
    docker build -t llm-agent .
    ```

2. Run the Docker container:

    ```sh
    docker run -p 8000:8000 llm-agent
    ```

## API Endpoints

- `POST /run`: Run a task based on the provided description.
- `GET /read`: Read the content of a file specified by the path.

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.
