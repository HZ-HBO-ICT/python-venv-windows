# Python Virtual Environment Setup (Windows)

This guide explains how to install Python on Windows, verify the installation, create a project, set up a virtual environment, and understand what a virtual environment does and why it is useful.

---

## What Is Python?

Python is a popular programming language used for web development, automation, data analysis, machine learning, and more.

---

## What Is a Virtual Environment?

A **virtual environment (venv)** is an isolated Python environment created for a specific project.

It contains:
- Its own Python interpreter
- Its own installed packages (libraries)

### Why Virtual Environments Are Useful

Virtual environments help you:

- Avoid dependency conflicts between projects
- Use different versions of the same package
- Keep your system Python installation clean
- Reproduce the same setup on another machine

Without virtual environments, all projects share the same packages, which can lead to version conflicts.

---

## Step 1: Install Python on Windows

1. Download Python from:  
   https://www.python.org/downloads/windows/

2. Run the installer.
3. **Check the box** ✅ **Add Python to PATH**
4. Click **Install Now** and complete the installation.

---

## Step 2: Verify Python Installation

Open **Command Prompt** and run:

```bash
python --version

This should give you something like this:
Python 3.x.x

## Step 3: Verify pip Installation
- pip is Python’s package manager. It is installed automatically with Python.
- pip --version

It should look something like this:
- pip x.x.x from C:\Python\Lib\site-packages\pip (python 3.x)

## Step 4: Create a Project Directory
Navigate to where you want your project and create a folder:

cd my_project

In your command line you should be in your project like this:
C:\path\to\my_project>

## Step 5: Create a Virtual Environment
python -m venv venv

A folder called venv should be added to the project folder

## Step 6: Activate the Virtual Environment
venv\Scripts\activate

In your command line the path should look like this:
(venv) C:\path\to\my_project>

## Step 7: Install the needed libraries
You can do this by installing them seperately with commands like:
pip isntall pandas

Or you can do this by installing all of them from a requirements.txt

pip install -r requirements.txt