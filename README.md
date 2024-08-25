# Research Paper Search and Q&A

This repository provides a tool that allows users to search for a specified number of arXiv research papers on a given topic, store them in a Qdrant vector database, and then ask questions about those research papers.

## Features

- **Search arXiv Research Papers:** Users can search for research papers on a specific topic.
- **Store Papers in Qdrant:** The retrieved papers are stored in a Qdrant vector database for efficient retrieval.
- **Question Answering:** Users can ask questions about the stored research papers, and the system will provide answers based on the content of those papers.

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/research-paper-search-qa.git
   cd research-paper-search-qa
    ```
2. **Create a virtual environment and activate it:**

   ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```
   
3. **Install the required dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

## Configuration

Update the config.py file with your specific configuration settings, including Qdrant client details and embedding function.

## Usage

1. Start the Gradio UI:

   python src/index.py

2. Search for Papers:
   - Enter a topic in the UI to search for research papers.
   - The system will download the papers and store them in the Qdrant vector database.

3. Ask Questions:
   - Enter your question in the UI.
   - The system will retrieve relevant information from the stored papers and provide an answer.

## Dependencies

- Python
- Gradio
- LangChain
- Qdrant
- Other dependencies listed in requirements.txt

## License

This project is licensed under the MIT License. See the LICENSE file for more details.

## Acknowledgements

- LangChain
- Qdrant
- Gradio

For any issues or contributions, please open an issue or submit a pull request on GitHub.