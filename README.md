# RAG-based AI Agent
This project is a RAG (Retrieval-Augmented Generation) based AI agent that uses Ollama and Llama Index to interact with PDF files and code files. The agent leverages open-source LLMs (Large Language Models) to generate responses based on the tools provided to the LLMs.

## Project Structure
- `code_ready.py`: Contains functions to read and parse code files.
- `data/`: Directory containing PDF files and code files for the agent to process.
- `main.py`: The main script to run the AI agent.
- `output/`: Directory to store the generated code files.
- `prompts.py`: Contains prompt templates and context for the agent.
- `requirements.txt`: List of required packages to run the project.

## Setup
1. Clone the Repository:  
```
git clone https://github.com/MarshallOkafor/AI-agent.git
cd AI-agent
```
2. Create a Virtual Environment:  
```
python3 -m venv venv
source venv/bin/activate
```
3. Install Dependencies:
```
pip install -r requirements.txt
```
4. Run the Agent:
```
python main.py
```

## Usage
### Running the Agent
The main script `main.py` initializes the AI agent with the necessary tools and starts an interactive prompt session where users can input queries. The agent processes the queries and provides code generation and analysis based on the given context and tools.

### File Structure
**PDF and Code Files**: Place your PDF and code files in the `data/` directory. The agent will read and process these files.
**Output Files**: The generated code files will be saved in the output/ directory.

### Example
1. Start the agent:
```
python main.py
```
2. Enter a prompt:
```
Enter a prompt (q to quit): Generate a Python function to read a text file.
```
3. View the generated code and description:
```
Code generated
def read_text_file(file_path):
    with open(file_path, 'r') as file:
        return file.read()

Description: This function reads the content of a text file given its file path.

Saved file: read_text_file.py
```
## License
This project is licensed under the MIT License. See the LICENSE file for details.
