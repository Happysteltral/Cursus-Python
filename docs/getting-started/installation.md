# Installing Python

Before you can start programming in Python, you need to install it on your computer.

## Download Python

### Windows

1. Visit [python.org](https://www.python.org/downloads/)
2. Click "Download Python" (latest version)
3. Run the installer
4. **Important**: Check "Add Python to PATH" during installation
5. Click "Install Now"

### macOS

Option 1: Using the official installer
1. Visit [python.org](https://www.python.org/downloads/)
2. Download the macOS installer
3. Run the installer and follow the prompts

Option 2: Using Homebrew (recommended)
```bash
brew install python3
```

### Linux

Most Linux distributions come with Python pre-installed. To check:

```bash
python3 --version
```

If not installed, use your package manager:

**Ubuntu/Debian:**
```bash
sudo apt update
sudo apt install python3 python3-pip
```

**Fedora:**
```bash
sudo dnf install python3 python3-pip
```

## Verify Installation

Open a terminal or command prompt and type:

```bash
python3 --version
```

You should see something like:
```
Python 3.11.0
```

## Installing a Code Editor

You'll need a code editor to write Python code. Here are some popular options:

### Visual Studio Code (Recommended)

1. Download from [code.visualstudio.com](https://code.visualstudio.com/)
2. Install the Python extension from the Extensions marketplace
3. Configure the Python interpreter

### Other Options

- **PyCharm**: Full-featured IDE specifically for Python
- **Sublime Text**: Lightweight and fast
- **Atom**: Open-source and customizable
- **Jupyter Notebook**: Great for data science and learning

## Setting Up a Virtual Environment

Virtual environments help you manage project dependencies. Create one with:

```bash
# Create a virtual environment
python3 -m venv myenv

# Activate it (Windows)
myenv\Scripts\activate

# Activate it (macOS/Linux)
source myenv/bin/activate
```

## Your First Python Program

Create a file called `hello.py` and add:

```python
print("Hello, World!")
```

Run it:
```bash
python3 hello.py
```

You should see:
```
Hello, World!
```

Congratulations! You've successfully installed Python and run your first program!

## Next Steps

Now that you have Python installed, you're ready to start learning! Head over to [Python Basics](../course/basics.md) to begin.
