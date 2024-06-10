# Investment Opinion

This project fetches news headlines from various RSS feeds, summarizes them using the OpenAI API, and saves the summaries to a markdown file. The file is then pushed to a GitHub repository.

## Features

- Fetches news headlines from multiple RSS feeds.
- Summarizes news headlines using OpenAI's GPT-4o model.
- Saves the summaries to a markdown file in an export directory.
- Pushes the markdown file to a GitHub repository.

## Prerequisites

- Python 3.6 or higher
- Git
- OpenAI API
- GitHub account and corresponding repository

## Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/LymboGroove/InvestOpinion_GPT.git
    cd InvestOpinion_GPT
    ```

2. **Set up a virtual environment:**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. **Install the required Python libraries:**

    ```bash
    pip install feedparser openai gitpython
    ```

4. **Set up the local Git repository in the export folder:**

    ```bash
    mkdir export
    cd export
    git init
    git remote add origin https://github.com/LymboGroove/InvestOpinion_GPT.git
    cd ..
    ```

## Usage

1. **Configure your API keys and repository path.**

2. **Run the script:**

    ```bash
    python InvestOpinion.py
    ```

    The script will:
    - Fetch news headlines from the specified RSS feeds.
    - Summarize the headlines using the OpenAI API.
    - Save the summaries to a markdown file in the `export` folder.
    - Push the markdown file to the GitHub repository.

## Project Structure
├── export/                     # Directory where markdown files are saved
├── summarize_news.py           # Main script
├── README.md                   # Project documentation
└── venv/                       # Virtual environment (not included in the repository)

## Contributing

1. **Fork the repository:**

    ```bash
    git clone https://github.com/LymboGroove/InvestOpinion_GPT.git
    cd InvestOpinion_GPT
    ```

2. **Create a new branch for your feature:**

    ```bash
    git checkout -b new-branch
    ```

3. **Make your changes and commit them:**

    ```bash
    git add .
    git commit -m "Add your commit message"
    ```

4. **Push to your branch:**

    ```bash
    git push origin new-branch
    ```

5. **Create a pull request:**

    Go to the repository on GitHub and create a pull request.

## License

This project is licensed under the MIT License.