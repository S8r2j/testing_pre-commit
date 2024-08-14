# Pre-commit Hook Setup and Testing Guide

This guide will help you set up and test the pre-commit hooks in your project. Follow the steps below to ensure that your code adheres to the defined standards before committing.

## Prerequisites

- Ensure that you have Python installed on your system.
- Clone the repository and navigate to the project’s root directory.

## Setup Instructions and Testing in a Single Script

1. **Clone the Repository, Set Up the Virtual Environment, Install Requirements, and Test Pre-commit**

   You can run the following commands in your terminal to complete the entire process:

   ```bash
   # Clone the repository
   git clone <repository-url>
   cd <repository-directory>

   # Set up the virtual environment
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

   # Install the required packages
   pip install -r requirements.txt

   # Install pre-commit hooks
   pre-commit install

   # Modify the main.py file by adding the whitespaces randomly and consecutive 10 new lines

   # Add changes, commit, and push
   git add .
   git commit -m "Testing pre-commit"
   git push origin <branch-name>

   # You will see the outcome of the pre-commit in your terminal and at last check the status of the files
   git status
