# dev_setup
This repo shares the steps required to setup your laptop to run the automation in this repo.


Setting up a virtual environment in Python is a straightforward process and is useful for managing dependencies for different projects. Here's a step-by-step guide:

### 1. **Install Python (if not already installed)**

   - **Windows**: Download and install Python from [python.org](https://www.python.org/downloads/). Make sure to check the option to "Add Python to PATH" during installation.
   - **macOS**: Python comes pre-installed, but you can install the latest version using Homebrew with the command `brew install python`.
   - **Linux**: Python is usually pre-installed. If not, you can install it using your package manager, e.g., `sudo apt-get install python3`.

### 2. **Install `virtualenv` (optional but recommended)**

   You can use Python's built-in `venv` module or install `virtualenv` for more features.

   - To install `virtualenv`, run:
     ```
     pip3 install virtualenv
     ```

### 3. **Create a Virtual Environment**

   Navigate to your project directory and create a virtual environment. You can name the environment folder whatever you like, typically `venv` or `env`.

   - **Using `venv` (built-in):**
     ```
     python3 -m venv venv
     ```
   - **Using `virtualenv` (if installed):**
     ```
     virtualenv venv
     ```

### 4. **Activate the Virtual Environment**

   Once the virtual environment is created, you need to activate it:

   - **Windows:**
     ```
     venv\Scripts\activate
     ```
   - **macOS and Linux:**
     ```
     source venv/bin/activate
     ```

   After activation, your command prompt should show the name of the virtual environment, indicating that it's active.

### 5. **Install Dependencies**

   With the virtual environment activated, you can install your project's dependencies using `pip`:

   ```
   pip install <package-name>
   ```

   You can also install all dependencies listed in a `requirements.txt` file:

   ```
   pip install -r requirements.txt
   ```

### 6. **Deactivate the Virtual Environment**

   When you're done working in the virtual environment, you can deactivate it with:

   ```
   deactivate
   ```

This returns your shell to the normal Python environment.
