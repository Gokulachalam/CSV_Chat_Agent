## Chat-With_CSV


This repository contains a Streamlit web application that enables users to interactively query information from a CSV file. Users can upload a CSV file, pose questions related to the document, and receive answers based on the content of the file. The application utilizes OpenAI language models for natural language understanding and interaction.


## Demo








## Table of Contents

- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Usage](#usage)
- [Code Structure](#code-structure)
- [Configuration](#configuration)
- [Acknowledgments](#acknowledgments)
- [License](#license)

## Getting Started

Follow these instructions to set up and run the application locally.

### Prerequisites

Make sure you have the following dependencies installed:

- Python 3.7 or later
- pip (Python package installer)

### Installation

1. Clone the repository to your local machine:

    ```bash
    git clone https://github.com/your-username/chat-with-csv.git
    ```

2. Navigate to the project directory:

    ```bash
    cd chat-with-csv
    ```

3. Install the required Python packages:

    ```bash
    pip install -r requirements.txt
    ```

### Usage

1. Run the Streamlit application:

    ```bash
    streamlit run app.py
    ```

2. Open your web browser and go to the provided local URL (typically http://localhost:8501).

3. Upload a CSV file using the file uploader.

4. Enter a question related to the document in the text area.

5. Click the "Submit" button to get an answer based on the content of the CSV file.

## Code Structure

### `app.py`

This file contains the Streamlit web application code. Users interact with the application through a web interface, upload CSV files, ask questions, and receive answers.

### `utils.py`

This file contains utility functions, specifically the `get_answer_csv` function, which processes the CSV file and queries it using OpenAI language models.

### `secrets.toml`

This file is used to store sensitive information, such as API keys. Ensure that you have the required API key for OpenAI and uncomment the relevant line in `utils.py`.

## Configuration

Before running the application, make sure to configure the API key for OpenAI in `secrets.toml`. Uncomment the relevant line in `utils.py` and replace `"YOUR_API_KEY"` with your actual API key.

```toml
# secrets.toml
[openai]
api_key = "YOUR_API_KEY"
```

## Acknowledgments

Streamlit: An open-source Python library for creating web applications with minimal effort.
OpenAI: Providing powerful natural language processing models for various applications.


