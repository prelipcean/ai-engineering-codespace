# ai-engineering-codespace

AI engineering

## Environment Setup

This project uses `uv` for fast Python package management and environment resolution. 

First, install `uv`:
```bash
pip install uv
```

*(Optional)* Clean up your terminal prompt for readability:
```bash
PS1="> "
```

Initialize the project and add the essential dependencies (this will set up your environment and install the required packages):
```bash
uv init
uv add python-dotenv jupyter openai
```

## VS Code Local Configuration

When opening this GitHub Codespace locally in VS Code, follow these steps to configure your workspace:

### 1. Select the Python Environment and Kernel
To ensure VS Code uses the correct dependencies installed by `uv`:
1. Open any `.ipynb` notebook or `.py` file.
2. Click the **Select Kernel** (for notebooks, top right) or **Python Environment** (for scripts, bottom right status bar) button.
3. Select the Python interpreter associated with this project's environment.
4. If prompted by VS Code, install any required Jupyter dependencies for the kernel.

### 2. Enable Automatic `.env` File Loading
To ensure your environment variables (like API keys) are automatically loaded when you open an integrated terminal:

1. Open VS Code Settings using the shortcut:
   - **Windows/Linux:** <kbd>Ctrl</kbd> + <kbd>,</kbd>
   - **macOS:** <kbd>Cmd</kbd> + <kbd>,</kbd>
2. In the top search bar, paste: `python.terminal.useEnvFile`
3. Look for **Python > Terminal: Use Env File** and check the box to turn it on.
4. Close your current terminal and open a new one for the changes to take effect.