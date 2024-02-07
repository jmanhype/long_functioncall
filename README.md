# Long Function Call Project

## Overview
This project is designed to process documents using the Haystack library for text processing and OpenAI's GPT models for natural language understanding. It converts files into a processed document format, stores them in a FAISSDocumentStore for quick retrieval, and uses an OpenAI model to extract structured data from the documents.

## Setup
To run this project, you will need Python 3.6 or higher. Clone the repository to your local machine and navigate to the cloned directory.

### Dependencies
- Haystack
- FAISSDocumentStore (part of the Haystack ecosystem)
- OpenAI's Python library
- Pandas
- SQLAlchemy
- PyYAML

### Configuration
Before running the scripts, you need to set up your OpenAI API key in an `apikeys.yml` file. Place this file in a directory that the script can access.

### Installation
Install the required Python packages using the following command:

```sh
pip install -r requirements.txt
```

This will install all the necessary libraries, including those needed for Haystack and OpenAI.

### Running the Script
To run the script, use the following command:

```sh
python long_function_call.ipynb
```

This will process the documents located in the `knowledge_base` directory, create a vector store for document retrieval, and execute function calls using the OpenAI API.

## Functionality
The script carries out the following main processes:
- Reads API keys from a configuration file.
- Pre-processes documents to convert them into a format suitable for Haystack's document store.
- Creates a FAISS vector store for efficient document retrieval.
- Uses OpenAI's GPT model to extract structured information from the documents.
- Updates a pandas DataFrame with the extracted information.

## How to Contribute
Contributions are welcome! If you have suggestions or improvements, please fork the repository and submit a pull request.

## License
Specify your project's license here, if applicable.

For more information on how to use the project or contribute, please refer to the individual script files and comments within the code.
