# jupyter-notebook-remote

## Environment Setup

### Prerequisites
- Python 3.10 or higher
- Poetry

### Installation

1. Install Poetry (if not already installed)
   ```bash
   curl -sSL https://install.python-poetry.org | python3 -
   poetry self update
   ```

2. Add Poetry to your PATH
   ```bash
   echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.bashrc
   source ~/.bashrc
   ```

3. Clone the repository
   ```bash
   git clone https://github.com/ishitsuka-hikaru/jupyter-notebook-remote.git
   cd jupyter-notebook-remote
   ```

4. Set up the environment with Poetry
   ```bash
   poetry install
   ```

## Usage

1. Start Jupyter Notebook
   ```bash
   poetry run jupyter notebook
   ```

2. Access the notebook in your browser
   - The server typically starts at `http://localhost:8888`
   - If port 8888 is in use, the server will automatically use another port
   - The security token is included in the URL, no additional input required

3. Shut down Jupyter Notebook
   - Press `Ctrl+C` twice in the terminal to stop the server

## Development

### Adding Dependencies
To add new Python packages to the project:
```bash
poetry add package-name
```

### Updating Dependencies
To update all dependencies to their latest versions:
```bash
poetry update
```