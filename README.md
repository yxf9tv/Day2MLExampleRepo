# My Project

A new Python project initialized with a virtual environment and best practices.

## Project Overview

This project provides a clean, organized structure for Python development with isolated dependencies and version control.

## Project Structure

```
├── venv/                # Python virtual environment
├── src/                 # Source code directory
├── tests/               # Test suite
├── data/                # Data files directory
├── main.py              # Main entry point
├── requirements.txt     # Python dependencies
├── .gitignore          # Git ignore rules
└── README.md           # This file
```

## Setup Instructions

### Prerequisites
- Python 3.10 or higher
- pip package manager

### Installation

1. **Clone the repository:**
   ```bash
   git clone <repo-url>
   cd MLDay2ExampleRepo
   ```

2. **Create and activate the virtual environment:**
   ```bash
   python3 -m venv venv
   ```
3. **Activate the virtual environment:**
   - **macOS/Linux:**
     ```bash
     source venv/bin/activate
     ```
   - **Windows:**
     ```bash
     venv\Scripts\activate
     ```

4. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

### Running the Project

Execute the main script:
```bash
python main.py
```

### Adding New Packages

1. Install the package:
   ```bash
   pip install package_name
   ```

2. Update requirements.txt:
   ```bash
   pip freeze > requirements.txt
   ```

3. Commit changes to version control:
   ```bash
   git add requirements.txt
   git commit -m "Add package_name to dependencies"
   ```

## Development Workflow

- Add source code in `src/`
- Write tests in `tests/`
- Store data files in `data/`
- Main entry point: `main.py`

## Environment Verification

To verify your virtual environment is correctly isolated:
```bash
which python  # Should show path within venv/
python -c "import sys; print(sys.prefix)"  # Should show venv directory
```

## Version Control

This project uses Git for version control. Key files are ignored:
- Virtual environment (`venv/`)
- Python cache files (`__pycache__/`)
- OS files (`.DS_Store`, etc.)

## Notes

- The virtual environment keeps project dependencies isolated from your system Python
- Always activate the virtual environment before working on the project
- Use `pip freeze > requirements.txt` to capture current dependencies

